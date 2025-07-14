

- Foundation
- StringTransform
-  latinToArabic 

Type Property

# latinToArabic

A constant containing the transliteration of a string from Latin script to Arabic script.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let latinToArabic: StringTransform
```

## Discussion

This transformation is reversible.

For example, the string “ạlʿarabīẗ‎” transliterates to “العَرَبِية”.

This is equivalent to kCFStringTransformLatinArabic.

## See Also

### Constants

static let latinToKatakana: StringTransform

A constant containing the transliteration of a string from Latin script to Katakana script.

static let latinToHiragana: StringTransform

A constant containing the transliteration of a string from Latin script to Hiragana script.

static let latinToHangul: StringTransform

A constant containing the transliteration of a string from Latin script to Hangul script.

static let latinToHebrew: StringTransform

A constant containing the transliteration of a string from Latin script to Hebrew script.

static let latinToThai: StringTransform

A constant containing the transliteration of a string from Latin script to Thai script.

static let latinToCyrillic: StringTransform

A constant containing the transliteration of a string from Latin script to Cyrillic script.

static let toLatin: StringTransform

A constant containing the transliteration of a string from any script to Latin script.

static let mandarinToLatin: StringTransform

A constant containing the transliteration of a string from Han script to Latin.

static let hiraganaToKatakana: StringTransform

A constant containing the transliteration of a string from Hiragana script to Katakana script.

static let fullwidthToHalfwidth: StringTransform

A constant containing the transformation of a string from full-width CJK characters to half-width forms.

static let toXMLHex: StringTransform

A constant containing the transformation of a string from characters to XML hexadecimal escape codes.

static let toUnicodeName: StringTransform

An identifier for a transform that converts characters to Unicode names.

static let stripCombiningMarks: StringTransform

A constant containing the transformation of a string by removing combining marks.

static let stripDiacritics: StringTransform

A constant containing the transformation of a string by removing diacritics.

