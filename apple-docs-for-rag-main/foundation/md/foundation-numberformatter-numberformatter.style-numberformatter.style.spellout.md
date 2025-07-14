

- Foundation
- NumberFormatter
- NumberFormatter.Style
-  NumberFormatter.Style.spellOut 

Case

# NumberFormatter.Style.spellOut

A style format in which numbers are spelled out in the language defined by the number formatter locale.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case spellOut
```

## Discussion

For example, in the en_US locale, the number 1234.5678 is represented as one thousand two hundred thirty-four point five six seven eight; in the fr_FR locale, the number 1234.5678 is represented as mille deux cent trente-quatre virgule cinq six sept huit.

This style is supported for most user locales. If this style doesn’t support the number formatter locale, the en_US locale is used as a fallback.

## See Also

### Formatting Styles

case none

An integer representation.

case decimal

A decimal style format.

case percent

A percent style format.

case scientific

A scientific style format.

case ordinal

An ordinal style format.

case currency

A currency style format that uses the currency symbol defined by the number formatter locale.

case currencyAccounting

An accounting currency style format that uses the currency symbol defined by the number formatter locale.

case currencyISOCode

A currency style format that uses the ISO 4217 currency code defined by the number formatter locale.

case currencyPlural

A currency style format that uses the pluralized denomination defined by the number formatter locale.

case none

An integer representation.

case decimal

A decimal style format.

case percent

A percent style format.

case scientific

A scientific style format.

case ordinal

An ordinal style format.

case currency

A currency style format that uses the currency symbol defined by the number formatter locale.

