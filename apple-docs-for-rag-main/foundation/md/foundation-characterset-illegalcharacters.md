

- Foundation
- CharacterSet
-  illegalCharacters 

Type Property

# illegalCharacters

Returns a character set containing values in the category of Non-Characters or that have not yet been defined in version 3.2 of the Unicode standard.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var illegalCharacters: CharacterSet { get }
```

## See Also

### Getting Standard Character Sets

static var alphanumerics: CharacterSet

Returns a character set containing the characters in Unicode General Categories L\*, M\*, and N\*.

static var capitalizedLetters: CharacterSet

Returns a character set containing the characters in Unicode General Category Lt.

static var controlCharacters: CharacterSet

Returns a character set containing the characters in Unicode General Category Cc and Cf.

static var decimalDigits: CharacterSet

Returns a character set containing the characters in the category of Decimal Numbers.

static var decomposables: CharacterSet

Returns a character set containing individual Unicode characters that can also be represented as composed character sequences (such as for letters with accents), by the definition of “standard decomposition” in version 3.2 of the Unicode character encoding standard.

static var letters: CharacterSet

Returns a character set containing the characters in Unicode General Category L\* & M\*.

static var lowercaseLetters: CharacterSet

Returns a character set containing the characters in Unicode General Category Ll.

static var newlines: CharacterSet

Returns a character set containing the newline characters (`U+000A ~ U+000D`, `U+0085`, `U+2028`, and `U+2029`).

static var nonBaseCharacters: CharacterSet

Returns a character set containing the characters in Unicode General Category M\*.

static var punctuationCharacters: CharacterSet

Returns a character set containing the characters in Unicode General Category P\*.

static var symbols: CharacterSet

Returns a character set containing the characters in Unicode General Category S\*.

static var uppercaseLetters: CharacterSet

Returns a character set containing the characters in Unicode General Category Lu and Lt.

static var whitespaces: CharacterSet

Returns a character set containing the characters in Unicode General Category Zs and `CHARACTER TABULATION (U+0009)`.

static var whitespacesAndNewlines: CharacterSet

Returns a character set containing characters in Unicode General Category Z\*, `U+000A ~ U+000D`, and `U+0085`.

