

- Foundation
- NumberFormatter
- NumberFormatter.Style
-  NumberFormatter.Style.currencyISOCode 

Case

# NumberFormatter.Style.currencyISOCode

A currency style format that uses the ISO 4217 currency code defined by the number formatter locale.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case currencyISOCode
```

## Discussion

This style behaves like the NumberFormatter.Style.currency style, except that the currency symbol is replaced by the corresponding ISO 4217 currency code. For example, in the en_US locale, the number 1234.5678 is represented as USD1,234.57; in the fr_FR locale, the number 1234.5678 is represented as 1 234,57 EUR.

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

case spellOut

A style format in which numbers are spelled out in the language defined by the number formatter locale.

case ordinal

An ordinal style format.

case currency

A currency style format that uses the currency symbol defined by the number formatter locale.

case currencyAccounting

An accounting currency style format that uses the currency symbol defined by the number formatter locale.

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

case spellOut

A style format in which numbers are spelled out in the language defined by the number formatter locale.

case ordinal

An ordinal style format.

