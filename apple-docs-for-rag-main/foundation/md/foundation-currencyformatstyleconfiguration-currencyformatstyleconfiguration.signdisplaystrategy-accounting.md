

- Foundation
- CurrencyFormatStyleConfiguration
- CurrencyFormatStyleConfiguration.SignDisplayStrategy
-  accounting 

Type Property

# accounting

A sign display strategy to use accounting principles.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var accounting: CurrencyFormatStyleConfiguration.SignDisplayStrategy { get }
```

## Discussion

This strategy always shows the currency symbol, and shows negative values in parenthesis. Examples of this strategy include `$123`, `$0`, and `($123)`.

## See Also

### Specifying sign display strategy

static var never: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A strategy to never show the sign.

static var automatic: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A strategy to automatically configure sign display.

static func accountingAlways(showZero: Bool) -> CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to use accounting principles, with a configurable behavior for handling zero values.

static func always(showZero: Bool) -> CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to always show the sign, with a configurable behavior for handling zero values.

