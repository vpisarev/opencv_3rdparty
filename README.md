# Unicode Font for OpenCV

The directory contains WenQuanYiMicroHei.ttf.gz compressed unicode font covering multiple scripts, including Latin, Cyrillic, Greek and CJK. This is the patched version of the font with proper "advance width" fields in Korean characters.

The font is distributed under Apache 2 license, see WQY_APL2.txt.
The font is builtin into OpenCV by default. If you experience problems with automatic download of the font by CMake script, download it manually and place it into `<opencv_build_directory>/modules/imgproc`. After downloading the font make sure that the checksum is correct and matches the one specified in `<opencv>/modules/imgproc/CMakeScripts.txt`.

Below is the original README, supplied with the font:

```
==========================================================

                 Wen Quan Yi Micro Hei

                    Release Notes

----------------------------------------------------------

Summary:

    Author   : WenQuanYi Project Contributors
    Webpage  : http://wenq.org/en/ or http://wqy.sourceforge.net/en/
    Font Name: WenQuanYi Micro Hei
    Version  : 0.2.0-beta (Big-Bang)
    Release  : 0
    Copyright  Digitized data copyright © 2007, Google Corporation.
               Copyright © 2008-2009, WenQuanYi Project Board of
               Trustees, All rights reserved.

               Droid Sans Fallback extension interface
               ( http://wenq.org/index.cgi?Fontopia(cn) ),
               copyright © 2008-2009 mozbug and Qianqian Fang
    License  : This font is licensed under Apache2.0 or GPLv3
               with font embedding exceptions (see Appendix B).
               Read LICENSE_Apache2.txt and LICENSE_GPLv3.txt for details

----------------------------------------------------------

Table of Content

 I.    About this font
 II.   Development History
 III.  Credits
 IV.   Language Coverage
 V.    About "WenQuanYi Project"
 VI.   Links
 VII.  Appendix

----------------------------------------------------------


 I. About this font

WenQuanYi Micro Hei font family is a Sans-Serif style (also known as Hei,
Gothic or Dotum among the Chinese/Japanese/Korean users) high quality
CJK outline font. It was derived from "Droid Sans Fallback", "Droid
Sans" and "Droid Sans Mono" released by Google Corp. This font package
contains two faces, "Micro Hei" and "Micro Hei Mono", in form of a
True-Type Collection (ttc) file. All the unified CJK Han glyphs, i.e.
GBK Hanzi, in the range of U+4E00-U+9FC3 defined in Unicode Standard 5.1
are covered, with additional support to many other international
languages such as Latin, Extended Latin, Hanguls and Kanas. The font
file is extremely compact (~5M) compared with most known CJK fonts.
As a result, it can be used for hand-held devices or embedded systems, or
used on PC with a significantly small memory footprint. Because both
font faces carry hinting and kerning instructions for Latin glyphs,
they are the excellent choices for desktop fonts.


 II. Development History

The original Droid Sans Fallback font contain 16,000 Unified Han glyphs,
and was officially released by Google under Apache2 license on Dec. 9,
2008 [2]. With a Javascript-based web interface, Fontopia(TM) [1], developed
by mozbug and Qianqian Fang, the WenQuanYi contributors had completed
over 10,000 new glyphs by combining the spline contours from the existing
Droid Han glyphs. By the end of 2008, project phase-1 had almost
completed, and phase-2 for CJK Extension A (U+3400-U+4DB5) was brought
online on Dec. 29, 2009. A review panel was formed to reinforce the
quality of all submitted glyphs [3]. In Jan. 2009, the reviewers
had redone over 2000 Hanzi and completed all the missing characters.
The nightly-build font has become online since Jan. 16. As of Feb. 2009, there
has been over 5500 CJK Extension A Han glyphs completed, which led this
font toward a complete GB18030 coverage.

In this font, we incorporated the high quality Latin glyphs from "Droid Sans"
and "Droid Sans Mono", which contain not only a better coverage but also
the additional hinting and kerning information. The EM of MicroHei
and MicroHeiMono fonts were unified to 2048 to retain all the advanced
typesetting features.


 III. Credits

We cordially thank Google(TM) for generously releasing Droid fonts to
public under an open-source license. Google purchased the font from
Ascenders Corp. (which was originally designed by a Chinese company).

The project for extending the Droid fonts is based on the web-based
glyph-composing applet [1], created by mozbug and Qianqian Fang
jointly. They are constantly improving this application targeting at
a web-based collaborative font development environment.

Over a thousand anonymous contributors have participated the project;
they submitted over 10,000 new Hanzi glyphs and many modifications.
The full update history of the glyphs can be found at [4].

The key members of the review panel, i.e. lsz, FangQ, kmc, Xhacker,
philacorns, and an "anonymous" (as requested) contributor, had
spent significant amount of efforts to redesign nearly half of the
submitted glyphs. We appreciate the incredible effort from this team
to make this font available. The detailed review credit can be found
at [3]


 IV.    Language Coverage

The following table is based on the locale data provided by fontconfig
(generated by langcover.pl from Dejavu Project
http://dejavu.sourceforge.net/wiki/index.php/Font_utilities).
  ----------------------------------------------------------------
    Locale                                           MicroHei
  ----------------------------------------------------------------
  aa     Afar                                     100% (62/62)
  ab     Abkhazia                                 100% (90/90)
  af     Afrikaans                                100% (69/69)
  am     Amharic                                       (0/264)
  ar     Arabic                                        (0/125)
  as                                                   (0/89)
  ast    Asturian                                 100% (72/72)
  ava    Avaric                                   100% (67/67)
  ay     Aymara                                   100% (60/60)
  az     Azerbaijani                               98% (146/148)
  az-ir  Azerbaijani in Iran                           (0/130)
  ba     Bashkir                                  100% (82/82)
  bam    Bambara                                   90% (54/60)
  be     Byelorussian                             100% (68/68)
  bg     Bulgarian                                100% (60/60)
  bh     Bihari (Devanagari script)                    (0/68)
  bho    Bhojpuri (Devanagari script)                  (0/68)
  bi     Bislama                                  100% (58/58)
  bin    Edo or Bini                              100% (78/78)
  bn     Bengali                                       (0/89)
  bo     Tibetan                                       (0/95)
  br     Breton                                   100% (64/64)
  bs     Bosnian                                  100% (62/62)
  bua    Buriat (Buryat)                          100% (70/70)
  ca     Catalan                                  100% (74/74)
  ce     Chechen                                  100% (67/67)
  ch     Chamorro                                 100% (58/58)
  chm    Mari (Lower Cheremis / Upper Cheremis)   100% (76/76)
  chr    Cherokee                                      (0/85)
  co     Corsican                                 100% (85/85)
  cs     Czech                                    100% (82/82)
  cu     Old Church Slavonic                      100% (103/103)
  cv     Chuvash                                  100% (74/74)
  cy     Welsh                                    100% (78/78)
  da     Danish                                   100% (70/70)
  de     German                                   100% (60/60)
  dz     Dzongkha                                      (0/95)
  el     Greek                                    100% (70/70)
  en     English                                  100% (73/73)
  eo     Esperanto                                100% (64/64)
  es     Spanish                                  100% (67/67)
  et     Estonian                                 100% (64/64)
  eu     Basque                                   100% (56/56)
  fa     Persian                                       (0/129)
  fi     Finnish                                  100% (63/63)
  fj     Fijian                                   100% (52/52)
  fo     Faroese                                  100% (68/68)
  fr     French                                   100% (85/85)
  ful    Fulah (Fula)                              87% (54/62)
  fur    Friulian                                 100% (66/66)
  fy     Frisian                                  100% (75/75)
  ga     Irish                                     82% (66/80)
  gd     Scots Gaelic                             100% (70/70)
  gez    Ethiopic (Geez)                               (0/218)
  gl     Galician                                 100% (66/66)
  gn     Guarani                                  100% (70/70)
  gu     Gujarati                                      (0/78)
  gv     Manx Gaelic                              100% (54/54)
  ha     Hausa                                     86% (52/60)
  haw    Hawaiian                                  98% (62/63)
  he     Hebrew                                        (0/27)
  hi     Hindi (Devanagari script)                     (0/68)
  ho     Hiri Motu                                100% (52/52)
  hr     Croatian                                 100% (62/62)
  hu     Hungarian                                100% (70/70)
  hy     Armenian                                      (0/77)
  ia     Interlingua                              100% (52/52)
  ibo    Igbo                                     100% (58/58)
  id     Indonesian                               100% (54/54)
  ie     Interlingue                              100% (52/52)
  ik     Inupiaq (Inupiak, Eskimo)                100% (68/68)
  io     Ido                                      100% (52/52)
  is     Icelandic                                100% (70/70)
  it     Italian                                  100% (73/73)
  iu     Inuktitut                                     (0/161)
  ja     Japanese                                  99% (6526/6538)
  ka     Georgian                                      (0/33)
  kaa    Kara-Kalpak (Karakalpak)                 100% (78/78)
  ki     Kikuyu                                   100% (56/56)
  kk     Kazakh                                   100% (77/77)
  kl     Greenlandic                              100% (81/81)
  km     Khmer                                         (0/70)
  kn     Kannada                                       (0/80)
  ko     Korean                                   100% (2443/2443)
  kok    Kokani (Devanagari script)                    (0/68)
  ks     Kashmiri (Devanagari script)                  (0/68)
  ku     Kurdish                                  100% (64/64)
  ku-ir  Kurdish in Iran                               (0/32)
  kum    Kumyk                                    100% (66/66)
  kv     Komi (Komi-Permyak/Komi-Siryan)          100% (70/70)
  kw     Cornish                                   96% (62/64)
  ky     Kirgiz                                   100% (70/70)
  la     Latin                                    100% (68/68)
  lb     Luxembourgish (Letzeburgesch)            100% (75/75)
  lez    Lezghian (Lezgian)                       100% (67/67)
  ln     Lingala                                   92% (75/81)
  lo     Lao                                           (0/65)
  lt     Lithuanian                               100% (70/70)
  lv     Latvian                                  100% (78/78)
  mg     Malagasy                                 100% (56/56)
  mh     Marshallese                              100% (62/62)
  mi     Maori                                     96% (62/64)
  mk     Macedonian                               100% (42/42)
  ml     Malayalam                                     (0/78)
  mn     Mongolian                                     (0/130)
  mo     Moldavian                                 98% (126/128)
  mr     Marathi (Devanagari script)                   (0/68)
  mt     Maltese                                  100% (72/72)
  my     Burmese (Myanmar)                             (0/48)
  nb     Norwegian Bokmal                         100% (70/70)
  nds    Low Saxon                                100% (59/59)
  ne     Nepali (Devanagari script)                    (0/68)
  nl     Dutch                                    100% (83/83)
  nn     Norwegian Nynorsk                        100% (76/76)
  no     Norwegian (Bokmal)                       100% (70/70)
  ny     Chichewa                                 100% (54/54)
  oc     Occitan                                  100% (70/70)
  om     Oromo or Galla                           100% (52/52)
  or     Oriya                                         (0/79)
  os     Ossetic                                  100% (66/66)
  pa     Punjabi (Gurumukhi script)                    (0/63)
  pl     Polish                                   100% (70/70)
  ps-af  Pashto in Afghanistan                         (0/49)
  ps-pk  Pashto in Pakistan                            (0/49)
  pt     Portuguese                               100% (83/83)
  rm     Rhaeto-Romance (Romansch)                100% (66/66)
  ro     Romanian                                  96% (60/62)
  ru     Russian                                  100% (66/66)
  sa     Sanskrit (Devanagari script)                  (0/68)
  sah    Yakut                                    100% (76/76)
  sco    Scots                                     92% (52/56)
  se     North Sami                               100% (66/66)
  sel    Selkup (Ostyak-Samoyed)                  100% (66/66)
  sh     Serbo-Croatian                           100% (76/76)
  si     Sinhala (Sinhalese)                           (0/77)
  sk     Slovak                                   100% (86/86)
  sl     Slovenian                                100% (62/62)
  sm     Samoan                                    98% (52/53)
  sma    South Sami                               100% (60/60)
  smj    Lule Sami                                100% (60/60)
  smn    Inari Sami                               100% (68/68)
  sms    Skolt Sami                                87% (70/80)
  so     Somali                                   100% (52/52)
  sq     Albanian                                 100% (56/56)
  sr     Serbian                                  100% (76/76)
  sv     Swedish                                  100% (68/68)
  sw     Swahili                                  100% (52/52)
  syr    Syriac                                        (0/45)
  ta     Tamil                                         (0/48)
  te     Telugu                                        (0/80)
  tg     Tajik                                    100% (78/78)
  th     Thai                                       1% (1/87)
  ti-er  Eritrean Tigrinya                             (0/256)
  ti-et  Ethiopian Tigrinya                            (0/282)
  tig    Tigre                                         (0/221)
  tk     Turkmen                                  100% (74/74)
  tl     Tagalog                                       (0/19)
  tn     Tswana                                   100% (56/56)
  to     Tonga                                     98% (52/53)
  tr     Turkish                                  100% (70/70)
  ts     Tsonga                                   100% (52/52)
  tt     Tatar                                    100% (76/76)
  tw     Twi                                       91% (67/73)
  tyv    Tuvinian                                 100% (70/70)
  ug     Uighur                                        (0/125)
  uk     Ukrainian                                100% (72/72)
  ur     Urdu                                          (0/145)
  uz     Uzbek                                    100% (68/68)
  ven    Venda                                     83% (52/62)
  vi     Vietnamese                                98% (191/194)
  vo     Volapuk                                  100% (54/54)
  vot    Votic                                    100% (62/62)
  wa     Walloon                                  100% (70/70)
  wen    Sorbian languages (lower and upper)      100% (76/76)
  wo     Wolof                                    100% (66/66)
  xh     Xhosa                                    100% (52/52)
  yap    Yapese                                   100% (58/58)
  yi     Yiddish                                       (0/27)
  yo     Yoruba                                    91% (109/119)
  zh-936                                           99% (21873/21920)
  zh-cn  Chinese (simplified)                      99% (6754/6765)
  zh-hk  Chinese Hong Kong Supplementary Character Set  99% (2212/2213)
  zh-mo  Chinese in Macau                          99% (2212/2213)
  zh-sg  Chinese in Singapore                      99% (6754/6765)
  zh-tw  Chinese (traditional)                     99% (13051/13063)
  zu     Zulu                                     100% (52/52)
  ----------------------------------------------------------------

 V.    About "WenQuanYi Project"

The "Wen Quan Yi" Project [5] was founded by Qianqian Fang [6] in
Oct. 2004. The goal of this project is to create a web-based
collaborative environment for open-source type-face development.
The initial focus of the project is to create high quality bitmap
character glyphs and outline fonts for all 70,000+ CJK characters
currently encoded by the Unicode Consortium. Some of the fonts
released by this project have been widely used as the default
Chinese desktop fonts by main-stream GNU/Linux distributions.

The Wen Quan Yi Project uses wiki [5] as the primary development
tool for glyph creation, documentation and coordinations. Wen Quan Yi
wiki also supports glyph version control and nightly build.


 VI.    Links

[1] http://wenq.org/index.cgi?Fontopia(cn)
[2] http://android.git.kernel.org/?p=platform/frameworks/base.git;a=commit;h=1a2
d9dbe9c6f54c5e0dc26386dc01df1d18073ad
[3] http://wenq.org/dev/index.cgi?BigBang_TASK
[4] http://wenq.org/WQYHistory.html.gz
[5] http://wenq.org/en/
[6] http://nmr.mgh.harvard.edu/~fangq/


 VII. Appendix

Appendix A.

Copyright disclaimer for UmeFont

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions
are met:
1. Redistributions of source code must retain the above copyright notice,
   this list of conditions and the following disclaimer.
2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.
3. Neither the name of the Wada Laboratory, the University of Tokyo nor
   the names of its contributors may be used to endorse or promote products
   derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY WADA LABORATORY, THE UNIVERSITY OF TOKYO AND
CONTRIBUTORS ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT
NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
PARTICULAR PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE LABORATORY OR
CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.


Appendix B.

GPL with font embedding exception:

http://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html#FontException

As a special exception, if you create a document which uses this
font, and embed this font or unaltered portions of this font into
the document, this font does not by itself cause the resulting
document to be covered by the GNU General Public License. This
exception does not however invalidate any other reasons why the
document might be covered by the GNU General Public License. If you
modify this font, you may extend this exception to your version of
the font, but you are not obligated to do so. If you do not wish to
do so, delete this exception statement from your version.
```
