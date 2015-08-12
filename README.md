## SignWriting Character Viewer
- - - 
> Version 1.0  
August 12th, 2015

The SignWriting Character Viewer shows all of the symbols of the International SignWriting Alphabet 2010 using any of the 4 different character encoding forms to access the glyphs of the [SignWriting 2010 Fonts][29].

The SignWriting Character Viewer is composed of an HTML file, a CSS file, and 5 JavaScript files.  For convenience, these files have been combined into a single file that is just over 100 KB.
* [SignWriting Character Viewer as single file][68]
* [SignWriting Character Viewer as multiple files][67]


### Character Encoding Forms
Symbol Keys  
S10000..S38b07; ISWA 2010 Symbol Keys  
ASCII characters, UTF-8 compatible.  
[Symbol keys][19] used as glyph names in the font files.

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

The character encodings used in SignWriting 2010 are defined in an Internet Draft submitted to the IETF: [draft-slevinski-signwriting-text][26].
The document is improved and resubmitted every 6 months.
The character design has been stable since January 12, 2012.
The current version of the Internet Draft is 05.
The next version is planned for November 2015.

- - -

Epilogue
----------
Feedback, bug reports, and patches are welcomed.

- - -

Version History
------------------
* 1.0 - Aug 12th, 2015: initial release

[19]: http://signbank.org/iswa
[26]: http://tools.ietf.org/html/draft-slevinski-signwriting-text
[29]: https://github.com/Slevinski/signwriting_2010_fonts
[60]: https://github.com/Slevinski/sw10js
[64]: http://www.unicode.org/versions/Unicode8.0.0/
[67]: https://slevinski.github.io/SignWriting_Character_Viewer/
[68]: https://slevinski.github.io/SignWriting_Character_Viewer/SignWriting_Character_Viewer.html