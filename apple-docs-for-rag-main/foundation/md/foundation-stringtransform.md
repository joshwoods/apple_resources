

- Foundation
-  StringTransform 

Structure

# StringTransform

Constants representing an ICU string transform.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct StringTransform
```

## Discussion

These constants are used by the NSString method applyingTransform(_:reverse:).

## Topics

### Transliteration

static let toLatin: StringTransform

A constant containing the transliteration of a string from any script to Latin script.

static let latinToArabic: StringTransform

A constant containing the transliteration of a string from Latin script to Arabic script.

static let latinToCyrillic: StringTransform

A constant containing the transliteration of a string from Latin script to Cyrillic script.

static let latinToGreek: StringTransform

A constant containing the transliteration of a string from Latin script to Greek script.

static let latinToHangul: StringTransform

A constant containing the transliteration of a string from Latin script to Hangul script.

static let latinToHebrew: StringTransform

A constant containing the transliteration of a string from Latin script to Hebrew script.

static let latinToHiragana: StringTransform

A constant containing the transliteration of a string from Latin script to Hiragana script.

static let latinToKatakana: StringTransform

A constant containing the transliteration of a string from Latin script to Katakana script.

static let latinToThai: StringTransform

A constant containing the transliteration of a string from Latin script to Thai script.

static let hiraganaToKatakana: StringTransform

A constant containing the transliteration of a string from Hiragana script to Katakana script.

static let mandarinToLatin: StringTransform

A constant containing the transliteration of a string from Han script to Latin.

### Diacritic and Combining Mark Removal

static let stripDiacritics: StringTransform

A constant containing the transformation of a string by removing diacritics.

static let stripCombiningMarks: StringTransform

A constant containing the transformation of a string by removing combining marks.

### Halfwidth and Fullwidth Form Conversion

static let fullwidthToHalfwidth: StringTransform

A constant containing the transformation of a string from full-width CJK characters to half-width forms.

### Character Representation

static let toUnicodeName: StringTransform

An identifier for a transform that converts characters to Unicode names.

static let toXMLHex: StringTransform

A constant containing the transformation of a string from characters to XML hexadecimal escape codes.

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Transforming Strings

func applyingTransform(StringTransform, reverse: Bool) -> String?

Returns a new string by applying a specified transform to the string.

