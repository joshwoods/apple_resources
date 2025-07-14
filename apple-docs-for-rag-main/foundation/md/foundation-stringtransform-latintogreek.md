

- Foundation
- StringTransform
-  latinToGreek 

Type Property

# latinToGreek

A constant containing the transliteration of a string from Latin script to Greek script.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let latinToGreek: StringTransform
```

## Discussion

This transformation is reversible.

For example, the string “Ellēnikó alphábēto‎” transliterates to “Ελληνικό αλφάβητο”.

This is equivalent to kCFStringTransformLatinGreek.

## See Also

### Transliteration

static let toLatin: StringTransform

A constant containing the transliteration of a string from any script to Latin script.

static let latinToArabic: StringTransform

A constant containing the transliteration of a string from Latin script to Arabic script.

static let latinToCyrillic: StringTransform

A constant containing the transliteration of a string from Latin script to Cyrillic script.

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

