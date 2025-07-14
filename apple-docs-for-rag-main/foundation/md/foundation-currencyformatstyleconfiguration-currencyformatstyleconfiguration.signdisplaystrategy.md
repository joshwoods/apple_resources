

- Foundation
- CurrencyFormatStyleConfiguration
-  CurrencyFormatStyleConfiguration.SignDisplayStrategy 

Structure

# CurrencyFormatStyleConfiguration.SignDisplayStrategy

A structure used to configure sign display strategies for currency format styles.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SignDisplayStrategy
```

## Topics

### Specifying sign display strategy

static var never: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A strategy to never show the sign.

static var automatic: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A strategy to automatically configure sign display.

static var accounting: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to use accounting principles.

static func accountingAlways(showZero: Bool) -> CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to use accounting principles, with a configurable behavior for handling zero values.

static func always(showZero: Bool) -> CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to always show the sign, with a configurable behavior for handling zero values.

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

struct Presentation

A structure used to configure the presentation of currency format styles.

