

- Core Foundation
-  kCFStringTransformToUnicodeName 

Global Variable

# kCFStringTransformToUnicodeName

The identifier of a reversible transform to transliterate characters other than printable ASCII to their Unicode character name in braces.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFStringTransformToUnicodeName: CFString!
```

## Discussion

Examples include `"\N{AIRPLANE}"` for “✈” and `"\N{GREEK CAPITAL LETTER PSI}"` for “Ψ”.

Note

The result of a forward transformation delimits each Unicode name with enclosing curly braces and the leading character sequence `"\N"`. In some programming languages, `"\N{...}"` is used as an escape sequence for Unicode characters in strings and regular expressions; this isn’t supported in Swift or Objective-C. To perform the reverse transform of a string literal in Swift or Objective-C, escape the leading backslash (`"\\N{...}"`) for each Unicode name.

## See Also

### Constants

let kCFStringTransformStripCombiningMarks: CFString!

The identifier of a transform to strip combining marks (accents or diacritics).

let kCFStringTransformToLatin: CFString!

The identifier of a transform to transliterate all text possible to Latin script. Ideographs are transliterated as Mandarin Chinese.

let kCFStringTransformFullwidthHalfwidth: CFString!

The identifier of a reversible transform to convert full-width characters to their half-width equivalents.

let kCFStringTransformLatinKatakana: CFString!

The identifier of a reversible transform to transliterate text to Katakana from Latin.

let kCFStringTransformLatinHiragana: CFString!

The identifier of a reversible transform to transliterate text to Hiragana from Latin.

let kCFStringTransformHiraganaKatakana: CFString!

The identifier of a reversible transform to transliterate text to Katakana from Hiragana.

let kCFStringTransformMandarinLatin: CFString!

The identifier of a transform to transliterate text to Latin from ideographs interpreted as Mandarin Chinese. This transform is not reversible.

let kCFStringTransformLatinHangul: CFString!

The identifier of a reversible transform to transliterate text to Hangul from Latin.

let kCFStringTransformLatinArabic: CFString!

The identifier of a reversible transform to transliterate text to Arabic from Latin.

let kCFStringTransformLatinHebrew: CFString!

The identifier of a reversible transform to transliterate text to Hebrew from Latin.

let kCFStringTransformLatinThai: CFString!

The identifier of a reversible transform to transliterate text to Thai from Latin.

let kCFStringTransformLatinCyrillic: CFString!

The identifier of a reversible transform to transliterate text to Cyrillic from Latin.

let kCFStringTransformLatinGreek: CFString!

The identifier of a reversible transform to transliterate text to Greek from Latin.

let kCFStringTransformToXMLHex: CFString!

The identifier of a reversible transform to transliterate characters other than printable ASCII to XML/HTML numeric entities.

let kCFStringTransformStripDiacritics: CFString!

The identifier of a transform to remove diacritic markings.

