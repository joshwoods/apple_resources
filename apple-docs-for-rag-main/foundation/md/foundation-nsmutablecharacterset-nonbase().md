

- Foundation
- NSMutableCharacterSet
-  nonBase() 

Type Method

# nonBase()

Returns a character set containing the characters in Unicode General Category M\*.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func nonBase() -> NSMutableCharacterSet
```

## See Also

### Getting Standard Character Sets

class func alphanumeric() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Categories L\*, M\*, and N\*.

class func capitalizedLetter() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category Lt.

class func control() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category Cc and Cf.

class func decimalDigit() -> NSMutableCharacterSet

Returns a character set containing the characters in the category of decimal numbers.

class func decomposable() -> NSMutableCharacterSet

Returns a character set containing individual Unicode characters that can also be represented as composed character sequences (such as for letters with accents), by the definition of “standard decomposition” in version 3.2 of the Unicode character encoding standard.

class func illegal() -> NSMutableCharacterSet

Returns a character set containing values in the category of Non-Characters or that have not yet been defined in version 3.2 of the Unicode standard.

class func letter() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category L\* & M\*.

class func lowercaseLetter() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category Ll.

class func newline() -> NSMutableCharacterSet

Returns a character set containing the newline characters (`U+000A` ~ `U+000D`, `U+0085`, `U+2028`, and `U+2029`).

class func punctuation() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category P\*.

class func symbol() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category S\*.

class func uppercaseLetter() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category Lu and Lt.

class func whitespaceAndNewline() -> NSMutableCharacterSet

Returns a character set containing characters in Unicode General Category Z\*, `U+000A` ~ `U+000D`, and `U+0085`.

class func whitespace() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category Zs and `CHARACTER TABULATION` (`U+0009`).

