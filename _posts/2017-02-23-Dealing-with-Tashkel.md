---
layout:     post
title:      "Dealing with Tashkel"
subtitle:   "FTS4 contentless and external content table"
date:       2017-02-23 17:00:00
author:     "Mohammad Yahia"
header-img: "img/posts/jekyll-bg.jpg"
comments: true
tags: [ Full_Text_Searchging ]
---
<span class="c5">بسم الله الرحمن الرحيم</span>

# <span class="c19">Introduction</span>

<span class="c5">The modern way for representing text characters is unicode (contrary to the old charsets),most modern programming languages and database systems support Unicode natively now</span>

<span class="c5">Sticking to the standard is the best practice to maintain portability and continuous improvement. So using the Unicode category is better than using manual function</span>

<span>Each unicode character is assigned a category, the arabic tashkeel characters are defined in</span> <span class="c24">['Mark, Nonspacing' category](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/category/Mn/index.htm&sa=D&ust=1499024386292000&usg=AFQjCNHSIgU3jA9N3fYK5sn2u3_yzm62zw)</span><span class="c5"> ‘Mn’</span>

## <span class="c14">Update:</span>

<span class="c5">A better way would be to leave only the letter,other {Lo} category which contains the basic arabic language</span>

<span class="c5">Also leave spaces,tabs and newlines</span>

<span class="c5">[^\p{Lo}\p{Z}\n]</span>

# <span class="c19">  
Arabic characters in the Mark,Nonspacing</span>

<span class="c5"></span>

<a id="t.f30ba60a6d7d0edf7a6db118d37c900912ecd13c"></a><a id="t.0"></a>

<table class="c40">

<tbody>

<tr class="c36">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0610](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0610/index.htm&sa=D&ust=1499024386293000&usg=AFQjCNEU89JaaQX_94RFoIIVdM91-V1wgQ)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SIGN SALLALLAHOU ALAYHE WASSALLAM</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ؐ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0610/arabic_sign_sallallahou_alayhe_wassallam.png&sa=D&ust=1499024386294000&usg=AFQjCNFTQ8hqSIJ3W3oTiI-WBY8qs5ISdA)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+0611](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0611/index.htm&sa=D&ust=1499024386294000&usg=AFQjCNFIYJ_-HYUs7rHpkPFEn96K1j630w)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SIGN ALAYHE ASSALLAM</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ؑ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0611/arabic_sign_alayhe_assallam.png&sa=D&ust=1499024386295000&usg=AFQjCNG-itJKeC_4RMO-YN-NcrRfgsLlxA)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0612](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0612/index.htm&sa=D&ust=1499024386295000&usg=AFQjCNHBjDpHD4ezH1VF3QhHAXfNRb4zcw)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SIGN RAHMATULLAH ALAYHE</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ؒ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0612/arabic_sign_rahmatullah_alayhe.png&sa=D&ust=1499024386296000&usg=AFQjCNFbthupn7n2zpe5-0NFzL39mjECsw)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+0613](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0613/index.htm&sa=D&ust=1499024386296000&usg=AFQjCNE91qVT29tUgEH4-Iy0vw0bJpCjNA)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SIGN RADI ALLAHOU ANHU</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ؓ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0613/arabic_sign_radi_allahou_anhu.png&sa=D&ust=1499024386297000&usg=AFQjCNFMwOSe2PjYWICojRCysYRgsn3QCA)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0614](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0614/index.htm&sa=D&ust=1499024386297000&usg=AFQjCNFSkAI3FY8671C0T4o5pP98WkWmnQ)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SIGN TAKHALLUS</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ؔ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0614/arabic_sign_takhallus.png&sa=D&ust=1499024386298000&usg=AFQjCNF0uGY4Col7a-UKlEZgX5mofYgQEA)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+0615](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0615/index.htm&sa=D&ust=1499024386298000&usg=AFQjCNFnp5Z1-F8p1uP-DbS7UsKIZjzEBw)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL HIGH TAH</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ؕ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0615/arabic_small_high_tah.png&sa=D&ust=1499024386299000&usg=AFQjCNE85BFNIcEJmtu9x676_ctsRo6LjQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0616](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0616/index.htm&sa=D&ust=1499024386300000&usg=AFQjCNEGi36JZNqbDX8_QJQb0lkB32j0gQ)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SMALL HIGH LIGATURE ALEF WITH LAM WITH YEH</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ؖ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0616/arabic_small_high_ligature_alef_with_lam_with_yeh.png&sa=D&ust=1499024386301000&usg=AFQjCNF3q5i6O0tNn4uE3lQRFIqDewrXjg)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+0617](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0617/index.htm&sa=D&ust=1499024386301000&usg=AFQjCNEdqkznvf0BfX4ilzYHJoBa9VIt4g)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL HIGH ZAIN</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ؗ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0617/arabic_small_high_zain.png&sa=D&ust=1499024386302000&usg=AFQjCNFkqI3-IH1UTooLjKan90ZU04obgA)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0618](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0618/index.htm&sa=D&ust=1499024386302000&usg=AFQjCNFgJAQGAknIjBNDphbWZYAJDQKJgw)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SMALL FATHA</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ؘ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0618/arabic_small_fatha.png&sa=D&ust=1499024386303000&usg=AFQjCNGclJKAHCO4SxI6OyvHOJN65AMOYw)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+0619](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0619/index.htm&sa=D&ust=1499024386303000&usg=AFQjCNE92QaPOOoKiq0fpbZ9jRUNqMC37A)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL DAMMA</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ؙ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0619/arabic_small_damma.png&sa=D&ust=1499024386304000&usg=AFQjCNGGJ1HNmyUtIExO3n4leDTxVK7X6Q)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+061A](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/061a/index.htm&sa=D&ust=1499024386304000&usg=AFQjCNF-bAO6Rs_pImR_uCjcWNdJCKlfZg)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SMALL KASRA</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ؚ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/061a/arabic_small_kasra.png&sa=D&ust=1499024386305000&usg=AFQjCNGzL8iWVlpM9bSoUBHh9DwQwvPjNA)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+064B](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/064b/index.htm&sa=D&ust=1499024386305000&usg=AFQjCNHkqoVkaTPnjLHN5kOlIKg_wsni_Q)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC FATHATAN</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ً</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/064b/arabic_fathatan.png&sa=D&ust=1499024386306000&usg=AFQjCNFs9wXw5HSV4u3ua0conYWn3rK8Rw)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+064C](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/064c/index.htm&sa=D&ust=1499024386306000&usg=AFQjCNH4Mw1lfsVlGz5cT46g0tm8mycw4w)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC DAMMATAN</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ٌ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/064c/arabic_dammatan.png&sa=D&ust=1499024386307000&usg=AFQjCNGwoz24M8yWPdnMoQrYTh6L_QvHZg)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+064D](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/064d/index.htm&sa=D&ust=1499024386307000&usg=AFQjCNGjnjER52fcOE_W2ZfW00j3fOkHxQ)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC KASRATAN</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ٍ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/064d/arabic_kasratan.png&sa=D&ust=1499024386308000&usg=AFQjCNH0t91ARjh9DBupIM7eEi5QaBE86g)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+064E](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/064e/index.htm&sa=D&ust=1499024386308000&usg=AFQjCNFocvWSrAg6fhQ3iEjb54ppF2Jtpw)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC FATHA</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">َ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/064e/arabic_fatha.png&sa=D&ust=1499024386309000&usg=AFQjCNGSOzAw_YF1sXHE3ovNqLe5xAkmwQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+064F](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/064f/index.htm&sa=D&ust=1499024386309000&usg=AFQjCNEmpQRGXFfgwGvQxlu3p6iLgOC2ag)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC DAMMA</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ُ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/064f/arabic_damma.png&sa=D&ust=1499024386310000&usg=AFQjCNFD_HU0OQqgf4p__6l8lbYC975-PQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0650](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0650/index.htm&sa=D&ust=1499024386310000&usg=AFQjCNH4VS2899KeugZ10fGVwOA5E2xN2g)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC KASRA</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ِ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0650/arabic_kasra.png&sa=D&ust=1499024386311000&usg=AFQjCNFltteucgGATAtStOcygs4cCqiZyQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+0651](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0651/index.htm&sa=D&ust=1499024386312000&usg=AFQjCNFTJDWDCnmMh3cS_1LIvTE90DF5rw)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SHADDA</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ّ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0651/arabic_shadda.png&sa=D&ust=1499024386312000&usg=AFQjCNHdaDm6QfsxF-g0xKZnDABwRrD2BA)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0652](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0652/index.htm&sa=D&ust=1499024386313000&usg=AFQjCNGUuzvdr6Twu_LNGz9NE1Gn4oXM_w)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SUKUN</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ْ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0652/arabic_sukun.png&sa=D&ust=1499024386313000&usg=AFQjCNGUGy1ueAaJvvej5S5m6LNKVJM82Q)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+0653](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0653/index.htm&sa=D&ust=1499024386314000&usg=AFQjCNHi132SMaKWLoi8ji98wXMgnIqEXA)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC MADDAH ABOVE</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ٓ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0653/arabic_maddah_above.png&sa=D&ust=1499024386314000&usg=AFQjCNHtI3lG4uwoIHIN5IapIt2Q8Wywdw)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0654](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0654/index.htm&sa=D&ust=1499024386315000&usg=AFQjCNGomqDG5VIJKSny0Za0N_fLuUBNcg)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c17 c18">ARABIC HAMZA ABOVE</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ٔ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0654/arabic_hamza_above.png&sa=D&ust=1499024386316000&usg=AFQjCNGddTJMw-ZOkZQ_vvkIX-2YcDq6Ew)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+0655](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0655/index.htm&sa=D&ust=1499024386316000&usg=AFQjCNH2zM9M_uPsS7Rek6jhOpiQLSdhTw)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC HAMZA BELOW</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ٕ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0655/arabic_hamza_below.png&sa=D&ust=1499024386317000&usg=AFQjCNFm8dyQtbBWq78SOyWNvDWs2SXhIA)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0656](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0656/index.htm&sa=D&ust=1499024386317000&usg=AFQjCNH4sQ6AxwF2NXHQZT7Bm0nGfBSBTA)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SUBSCRIPT ALEF</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ٖ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0656/arabic_subscript_alef.png&sa=D&ust=1499024386318000&usg=AFQjCNGmc99-AfuvcgehhY89_wFTZuIh7w)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+0657](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0657/index.htm&sa=D&ust=1499024386318000&usg=AFQjCNEkP_4VQQu3b3NQM-V7HWoUZUnJRw)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC INVERTED DAMMA</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ٗ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0657/arabic_inverted_damma.png&sa=D&ust=1499024386319000&usg=AFQjCNHV7LrInpR4eE3cCYHUYfmLMETC7A)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0658](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0658/index.htm&sa=D&ust=1499024386319000&usg=AFQjCNFH1d_UryP_ms66kXfUUNR_J42eFA)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC MARK NOON GHUNNA</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">٘</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0658/arabic_mark_noon_ghunna.png&sa=D&ust=1499024386320000&usg=AFQjCNGXV9BL8dfEsJnSh9BR3IbHQHg0Ew)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+0659](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0659/index.htm&sa=D&ust=1499024386320000&usg=AFQjCNEnJm-SaNQzbVsEaLk_nDMmq4zRvQ)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC ZWARAKAY</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ٙ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0659/arabic_zwarakay.png&sa=D&ust=1499024386321000&usg=AFQjCNElBvpN7SPbrQQuFZ5RkrUSYHoLiQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+065A](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065a/index.htm&sa=D&ust=1499024386321000&usg=AFQjCNENP4yGMDxATjxszbw380Sul6ylVA)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC VOWEL SIGN SMALL V ABOVE</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ٚ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065a/arabic_vowel_sign_small_v_above.png&sa=D&ust=1499024386322000&usg=AFQjCNEt6fniKSEoXZNylYzhYJNXoI1AOg)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+065B](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065b/index.htm&sa=D&ust=1499024386322000&usg=AFQjCNGt_6uDtHBrPQ9JrxeAUC5FGuJ_vQ)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC VOWEL SIGN INVERTED SMALL V ABOVE</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ٛ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065b/arabic_vowel_sign_inverted_small_v_above.png&sa=D&ust=1499024386323000&usg=AFQjCNEV_8F7z-9rPS0ghXkpL8cekFWF5Q)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+065C](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065c/index.htm&sa=D&ust=1499024386323000&usg=AFQjCNHH0sWImh-0ZiY2oad8xivCx1bq3g)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC VOWEL SIGN DOT BELOW</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ٜ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065c/arabic_vowel_sign_dot_below.png&sa=D&ust=1499024386324000&usg=AFQjCNFDk0a8p-Q4ciH-rGl63yj_jUJYBQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+065D](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065d/index.htm&sa=D&ust=1499024386324000&usg=AFQjCNEaKHDVqiAeF7Hl-maMX-ef5xV5gA)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC REVERSED DAMMA</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ٝ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065d/arabic_reversed_damma.png&sa=D&ust=1499024386325000&usg=AFQjCNFSVYQpZQanPCjlE6xN34cNP63POQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+065E](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065e/index.htm&sa=D&ust=1499024386325000&usg=AFQjCNFoq_f8Em193eSwszev2EWKpE7jog)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC FATHA WITH TWO DOTS</span>

</td>

<td class="c17 c20" colspan="1" rowspan="1">

<span class="c8">ٞ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065e/arabic_fatha_with_two_dots.png&sa=D&ust=1499024386326000&usg=AFQjCNHa9XnlMvWAlfJU_pU-0JB75ZDveA)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+065F](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065f/index.htm&sa=D&ust=1499024386326000&usg=AFQjCNG7ybOugBEcuiu16fgAWkWoNbtiRg)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC WAVY HAMZA BELOW</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ٟ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/065f/arabic_wavy_hamza_below.png&sa=D&ust=1499024386327000&usg=AFQjCNFUUJphZtowcnNK_XQIMk2hsD4O2Q)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+0670](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0670/index.htm&sa=D&ust=1499024386327000&usg=AFQjCNGBfBZMWNd0Y1HE1ZKrF-qq4Ywd9A)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC LETTER SUPERSCRIPT ALEF</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ٰ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/0670/arabic_letter_superscript_alef.png&sa=D&ust=1499024386328000&usg=AFQjCNEZbhgx7TR4qFfMUQxLUfFDyTRvYw)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+06D6](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06d6/index.htm&sa=D&ust=1499024386328000&usg=AFQjCNGL_YLvlRlVUO9pyghaWiMcORuEyA)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL HIGH LIGATURE SAD WITH LAM WITH ALEF MAKSURA</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ۖ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06d6/arabic_small_high_ligature_sad_with_lam_with_alef_maksura.png&sa=D&ust=1499024386329000&usg=AFQjCNE15u_AGaZaiqxhrH366BqLLi5sIg)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+06D7](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06d7/index.htm&sa=D&ust=1499024386329000&usg=AFQjCNGn71YaQ_phDUBlTF8JDr3aR6C--w)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SMALL HIGH LIGATURE QAF WITH LAM WITH ALEF MAKSURA</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ۗ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06d7/arabic_small_high_ligature_qaf_with_lam_with_alef_maksura.png&sa=D&ust=1499024386330000&usg=AFQjCNGXjOHG3ei3I8RCAR_w7SFHdLo7Nw)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+06D8](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06d8/index.htm&sa=D&ust=1499024386330000&usg=AFQjCNEFWJBY0emicJFZGDSV_Q_mVZav8w)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL HIGH MEEM INITIAL FORM</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ۘ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06d8/arabic_small_high_meem_initial_form.png&sa=D&ust=1499024386331000&usg=AFQjCNFJH_SZXFAhi0S-hLD2Dqz3HejY-w)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+06D9](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06d9/index.htm&sa=D&ust=1499024386331000&usg=AFQjCNEKZ2iOo3Uk5tqcbb4mz3BdClKPnw)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SMALL HIGH LAM ALEF</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ۙ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06d9/arabic_small_high_lam_alef.png&sa=D&ust=1499024386332000&usg=AFQjCNFQqYP_RxMCVUTkZSj5Kc8bo7g_-A)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+06DA](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06da/index.htm&sa=D&ust=1499024386332000&usg=AFQjCNH8weBJeVstTjdIaYQ4PLzJrTpJqw)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL HIGH JEEM</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ۚ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06da/arabic_small_high_jeem.png&sa=D&ust=1499024386333000&usg=AFQjCNF313x50YHTnuQBDZgouq_uwv2LQw)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+06DB](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06db/index.htm&sa=D&ust=1499024386333000&usg=AFQjCNEND3tCYT-DpJWDk4cGhFkSwr3Vhg)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SMALL HIGH THREE DOTS</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ۛ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06db/arabic_small_high_three_dots.png&sa=D&ust=1499024386334000&usg=AFQjCNFLsGDV3WSP9e4-jnftJ7Y_GQvqsQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+06DC](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06dc/index.htm&sa=D&ust=1499024386334000&usg=AFQjCNH_GSuswfn_mPe9_ifyJ5xj2fg-Sg)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL HIGH SEEN</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ۜ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06dc/arabic_small_high_seen.png&sa=D&ust=1499024386335000&usg=AFQjCNH-siypnmMsm89iOMZqfpu1layLYA)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+06DF](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06df/index.htm&sa=D&ust=1499024386336000&usg=AFQjCNFYC4LMCzSdQ9g8neuTurghNIpesQ)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SMALL HIGH ROUNDED ZERO</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">۟</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06df/arabic_small_high_rounded_zero.png&sa=D&ust=1499024386336000&usg=AFQjCNH52JgblBwX8I-Rruz9b70ePA93bQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+06E0](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e0/index.htm&sa=D&ust=1499024386337000&usg=AFQjCNEqdUJFtWX8HRhnsRMgjOd7Fu-3qQ)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL HIGH UPRIGHT RECTANGULAR ZERO</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">۠</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e0/arabic_small_high_upright_rectangular_zero.png&sa=D&ust=1499024386337000&usg=AFQjCNEgaLrsEnoF-df7IqzXVQF0dteDGQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+06E1](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e1/index.htm&sa=D&ust=1499024386338000&usg=AFQjCNHd6qFq7b6TorBcMYjr4mipiRJlxg)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SMALL HIGH DOTLESS HEAD OF KHAH</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ۡ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e1/arabic_small_high_dotless_head_of_khah.png&sa=D&ust=1499024386338000&usg=AFQjCNFGuxAu6UxBATHB5gMaOnTdsG2lBw)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+06E2](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e2/index.htm&sa=D&ust=1499024386339000&usg=AFQjCNE6Ui8SB5TbuulyqfiutZqqnbjvew)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL HIGH MEEM ISOLATED FORM</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ۢ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e2/arabic_small_high_meem_isolated_form.png&sa=D&ust=1499024386339000&usg=AFQjCNHIlEd3Ojm_QPgHb24yakorrQGWbw)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+06E3](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e3/index.htm&sa=D&ust=1499024386340000&usg=AFQjCNGk0mdvFPbZlxZWqCi7CHppu3OyNg)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SMALL LOW SEEN</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ۣ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e3/arabic_small_low_seen.png&sa=D&ust=1499024386341000&usg=AFQjCNGrfRyTYv3gi_VUaKrypPPrAzhPgg)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+06E4](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e4/index.htm&sa=D&ust=1499024386341000&usg=AFQjCNEmqkRwgd_NPsu3kLwRRjSKnOrU1A)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL HIGH MADDA</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ۤ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e4/arabic_small_high_madda.png&sa=D&ust=1499024386342000&usg=AFQjCNGEO9fH5HTKxrVzaUzmbCSlYOx0jQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+06E7](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e7/index.htm&sa=D&ust=1499024386342000&usg=AFQjCNFCraHc9VbZtU4sxsE_m_ockc4kmA)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC SMALL HIGH YEH</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">ۧ</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e7/arabic_small_high_yeh.png&sa=D&ust=1499024386343000&usg=AFQjCNE2orNid33Pnk0Kc_xVC_tyRQBZ0A)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+06E8](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e8/index.htm&sa=D&ust=1499024386343000&usg=AFQjCNGGz9b6VFkDtJ6UThrJjGO1W2Svlw)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC SMALL HIGH NOON</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">ۨ</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06e8/arabic_small_high_noon.png&sa=D&ust=1499024386344000&usg=AFQjCNFJyv1Fl5baKlJh48oeEuriPlFMHw)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+06EA](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06ea/index.htm&sa=D&ust=1499024386344000&usg=AFQjCNE9YMDSS--_W8_qWpOUsfEXWsSMhg)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC EMPTY CENTRE LOW STOP</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">۪</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06ea/arabic_empty_centre_low_stop.png&sa=D&ust=1499024386345000&usg=AFQjCNERjtOLrSPcVg8praRibQ2awdH8EQ)</span>

</td>

</tr>

<tr class="c16">

<td class="c9" colspan="1" rowspan="1">

<span class="c13">[U+06EB](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06eb/index.htm&sa=D&ust=1499024386345000&usg=AFQjCNHSwk1jI5lEBZ4WcJijPsdQHqkT_w)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c1">ARABIC EMPTY CENTRE HIGH STOP</span>

</td>

<td class="c20" colspan="1" rowspan="1">

<span class="c4">۫</span>

</td>

<td class="c12" colspan="1" rowspan="1">

<span class="c13">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06eb/arabic_empty_centre_high_stop.png&sa=D&ust=1499024386346000&usg=AFQjCNGzjB4FfOsDx_OT-XIbYyM36GvZQg)</span>

</td>

</tr>

<tr class="c16">

<td class="c6" colspan="1" rowspan="1">

<span class="c13 c17">[U+06EC](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06ec/index.htm&sa=D&ust=1499024386346000&usg=AFQjCNFeuHf1EYOnuJzQiff9UF4T_koTNg)</span>

</td>

<td class="c3 c17" colspan="1" rowspan="1">

<span class="c18 c17">ARABIC ROUNDED HIGH STOP WITH FILLED CENTRE</span>

</td>

<td class="c20 c17" colspan="1" rowspan="1">

<span class="c8">۬</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c13 c17">[view](https://www.google.com/url?q=http://www.fileformat.info/info/unicode/char/06ec/arabic_rounded_high_stop_with_filled_centre.png&sa=D&ust=1499024386347000&usg=AFQjCNHuAzfGT2J99ZM9pIQBQge_cCyQyw)</span>

</td>

</tr>

</tbody>

</table>

<span class="c5"></span>

# <span class="c19">Note about unicode representation (why normalization is not applicable)</span>

<span>The above shows that the unicode doesn’t have combined characters for Arabic language,had it done this searching could have been easier using the standard</span> <span class="c24">[normalization and canonical character equivlance](https://www.google.com/url?q=https://en.wikipedia.org/wiki/Unicode_equivalence&sa=D&ust=1499024386348000&usg=AFQjCNHe8XKKO2VovhsfQhmv7zwBZAu_rg)</span><span class="c5">.</span>

<span>So for now (</span><span class="c11">أَ</span><span class="c5">) alef with fatha is considered two characters ,as a result if searching with ignoring tashkeel is required tashkeel needs to be removed using method other than normalization.</span>

<span class="c5"></span>

<span>I don’t know for now why was this design choice made in the unicode standard</span>

# <span>Java</span> <span class="c19">Regex handling</span>

<span class="c29">To match a single character belonging to the</span> <span class="c29 c31"><category></span><span class="c29">category with</span> <span class="c26">\p{</span><span class="c26 c31"><category></span><span class="c26">}</span><span class="c29">.</span>

<span>The pattern to find</span> <span class="c5">Mark,Nonspacing category is “\p{Mn}” (for java the backslash needs to be escaped inside the string quotation “\\p{Mn}” )</span>

<span class="c5"></span>
