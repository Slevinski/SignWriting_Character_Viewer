## SignWriting Character Viewer
- - - 
> Version 2.5.0  
September 6th, 2017

The SignWriting Character Viewer shows all of the symbols of the International SignWriting Alphabet 2010 using a variety of character encoding forms to access the glyphs of the [SignWriting 2010 Fonts][29].
 
The main index page contains links for both version 1 and 2.
The main index uses the SignWriting 2010 JavaScript library (7 KB zipped) to convert a live Formal SignWriting string into HTML, CSS, SVG and TTF.
 * [SignWriting Character Viewer Index][67]  
 * [Available as 2 KB each of CSS, HTML, and custom JavaScript at CodePen.io][88]  


The SignWriting Character Viewer versions 1 and 2 use HTML, CSS, and JavaScript with TrueType Font files for display.

### Version 2 Character Encoding Forms
 * [SignWriting Character Viewer v2][69]  

For the 2016 font development work, the font design has been streamlined to simplify the design 
to eliminate Private Use Area characters and eliminate the use of feature files with almost 100,000 ligature statements.
For 2017 font work, additional Unicode characters were added to complete the encoding of SignWriting text.

Symbol Keys  
S10000..S38b07; ISWA 2010 Symbol Keys  
ASCII characters, UTF-8 compatible.  
[Symbol keys][19] used as glyph names in the font files.

SignWriting in Unicode (SWU)
experimental encoding supported by the Center for Sutton Movement Writing, inc.  
Overwrites the Sutton SignWriting block and uses Plane 4.  
Codepoints used as glyph id in the font files.
Uses 1 character per symbol.

The characters conversions implementation can be found in the [Sutton SignWriting JavaScript Library][61] in the "SuttonSignWriting.js" file under functions "ssw.opt" and "ssw.uni".


### Version 1 Character Encoding Forms 
* [SignWriting Character Viewer v1][68]

The forms of Unicode 8 and PUA Plane 15 have been deprecated and should no longer be used.  PUA Plane 16 is still used for the "SignWriting 2010 Font" development.

Unicode 8  
1D800..1DAAF; Sutton SignWriting  
[Unicode 8][64] support without facial diacritic combining.  
Uses 1 to 3 characters per symbol.

PUA Plane 15  
FD800..FDFFF; SignWriting Text   
Private Use Area characters.  
Uses 3 characters per symbol.  Includes characters for structural markers and numbers.

PUA Plane 16  
100000...10FFFF; Symbol Code Points  
Private Use Area characters.  
Uses 1 character per symbol.


The characters conversions implementation can be found in the [SignWriting 2010 JavaScript Library][60] in the "sw10.js" file under functions "uni8" for Unicode 8, "pua" for SignWriting Text characters on plane 15, and "code" for symbol code point characters on plane 16.  

- - -

Reference
----------
The character encodings used in the SignWriting Character Viewer are defined in an Internet Draft submitted to the IETF: [draft-slevinski-formal-signwriting][27].
The document is improved and resubmitted every 6 months.
The ASCII character design has been stable since January 12th, 2012.
The Unicode character design has been stable since July 14th, 2017.

- - -

Epilogue
----------
Feedback, bug reports, and patches are welcomed.

- - -

Version History
------------------
* 2.5.0 - Sept 6th, 2017: updated v2 for SWU and new fonts
* 2.4.0 - Jul 9th, 2016: added cursor stub and function
* 2.3.1 - Jul 1st, 2016: fix for index page LR lanes
* 2.3 - Jul 1st, 2016: css for signtext
* 2.2 - Jun 29th, 2016: zoom slider
* 2.1 - Jun 29th, 2016: signtext and plane 4 headers
* 2.0 - Jun 28th, 2016: version 2 with Unicode 10 proposal on Plane 4
* 1.0 - Aug 12th, 2015: initial release with Unicode 8, Plane 15 characters, and Plane 16 characters.

[19]: http://signbank.org/iswa
[26]: http://tools.ietf.org/html/draft-slevinski-signwriting-text
[27]: http://tools.ietf.org/html/draft-slevinski-formal-signwriting
[29]: https://github.com/Slevinski/signwriting_2010_fonts
[60]: https://github.com/Slevinski/sw10js
[61]: https://github.com/Slevinski/SuttonSignWriting
[64]: http://www.unicode.org/versions/Unicode8.0.0/
[67]: https://slevinski.github.io/SignWriting_Character_Viewer/
[68]: https://slevinski.github.io/SignWriting_Character_Viewer/SignWriting_Character_Viewer.html
[69]: https://slevinski.github.io/SignWriting_Character_Viewer/SignWriting_Character_Viewer_2.html
[88]: http://codepen.io/Slevinski/full/XKRPzm/
