

- Foundation
- NumberFormatter
-  NumberFormatter.Style 

Enumeration

# NumberFormatter.Style

The predefined number format styles used by the numberStyle property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Style
```

## Overview

The table below provides examples of each formatting style for the U.S., France, and China.

| Style | en_US Locale | fr_FR Locale | zh_CN Locale |
|----|----|----|----|
| NumberFormatter.Style.none | 1235 | 1235 | 1235 |
| NumberFormatter.Style.decimal | 1,234.568 | 1 234,568 | 1,234.568 |
| NumberFormatter.Style.percent | 12% | 12 % | 12% |
| NumberFormatter.Style.scientific | 1.2345678E3 | 1,2345678E3 | 1.2345678E3 |
| NumberFormatter.Style.spellOut | one hundred twenty-three | cent vingt-trois | 一百二十三 |
| NumberFormatter.Style.ordinal | 3rd | 3e | 第3 |
| NumberFormatter.Style.currency | \$1,234.57 | 1 234,57 € | ￥1,234.57 |
| NumberFormatter.Style.currencyAccounting | (\$1,234.57) | (1 234,57 €) | (￥1,234.57) |
| NumberFormatter.Style.currencyISOCode | USD1,234.57 | 1 234,57 EUR | CNY1,234.57 |
| NumberFormatter.Style.currencyPlural | 1,234.57 US dollars | 1 234,57 euros | 1,234.57人民币 |

## Topics

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

case spellOut

A style format in which numbers are spelled out in the language defined by the number formatter locale.

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

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum Behavior

These constants specify the behavior of a number formatter. These constants are returned by the defaultFormatterBehavior() class method and the formatterBehavior property.

enum PadPosition

These constants are used to specify how numbers should be padded. These constants are used by the paddingPosition property.

enum RoundingMode

These constants are used to specify how numbers should be rounded. These constants are used by the roundingMode property.

