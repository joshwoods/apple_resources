

- Foundation
- CurrencyFormatStyleConfiguration
-  CurrencyFormatStyleConfiguration.Presentation 

Structure

# CurrencyFormatStyleConfiguration.Presentation

A structure used to configure the presentation of currency format styles.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Presentation
```

## Topics

### Specifying presentation

static var fullName: CurrencyFormatStyleConfiguration.Presentation

A presentation that shows the full name of the currency.

static var isoCode: CurrencyFormatStyleConfiguration.Presentation

A presentation that shows the ISO code of the currency.

static var narrow: CurrencyFormatStyleConfiguration.Presentation

A presentation that shows a condensed expression of the currency.

static var standard: CurrencyFormatStyleConfiguration.Presentation

A presentation that shows a standard expression of the currency.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Specifying Configuration

typealias Grouping

The type used to configure grouping for currency format styles.

typealias Precision

The type used to configure precision for currency format styles.

typealias DecimalSeparatorDisplayStrategy

The type used to configure decimal separator display strategies for currency format styles.

typealias RoundingRule

The type used to configure rounding rules for currency format styles.

struct SignDisplayStrategy

A structure used to configure sign display strategies for currency format styles.

