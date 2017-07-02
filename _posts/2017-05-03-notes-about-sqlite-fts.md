---
layout:     post
title:      "Notes about SqLite FTS3 and FTS4"
subtitle:   "FTS4 contentless and external content table"
date:       2017-05-03 17:00:00
author:     "Mohammad Yahia"
header-img: "img/posts/jekyll-bg.jpg"
comments: true
tags: [ Full_Text_Searchging ]
---
See [the documentation for the content option forr fts4 tables](https://www.sqlite.org/fts3.html#*fts4content) 
 
The way I choosed:
Using contentless table then joining with the table which contains the data
This way have :
- No data duplication
- FTS indexing only the needed coulmn

Using external content table would also save space and allow easier syntax for retrieving data but will also require join to get hte non-indexed coulmns (this would have been solved if android supports newer version of sqlite which allows notindexed option)
 
## creating the index
 
CREATE VIRTUAL TABLE pageTextSearch USING fts4(content="", page);
INSERT INTO pageTextSearch(docid,page) SELECT id,page from pages;
select pages.page,pages.id,pages.partnumber,pages.pagenumber ,searchResult.docid,matchedinfo
from pages
inner join
(select docid,matchinfo(pageTextSearch) as matchedinfo from pageTextSearch where pageTextSearch.page match "نَافِع") as searchResult
on pages.id=searchResult.docid
 
 
## FTS search 
select
searchResult.docid as searchResult_pageId,
pages.partnumber as searchResult_partnumber,
pages.pagenumber as searchResult_pagenumber,
pages.page as searchResult_page,
 
titles.id as parent_title_id,
titles.title as parent_title_title,
titles.pageid  as parent_title_pageid,
titlePage.pagenumber as parent_title_pagenumber,
titlePage.partnumber as parent_title_partnumber,
titlePage.page as parent_title_page
 
from
(SELECT docid FROM pageTextSearch WHERE page MATCH ?
)
as searchResult
join
titles
on
titles.pageid =(select max(titles.pageid) from titles where titles.pageid<=searchResult.docid)
join
pages
on
pages.id=searchResult.docid
join
pages as titlePage
on
titlePage.id=titles.pageid
 
order by pages.id
 
 
