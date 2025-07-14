

- Foundation
- CurrencyFormatStyleConfiguration
- CurrencyFormatStyleConfiguration.SignDisplayStrategy
-  never 

Type Property

# never

A strategy to never show the sign.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var never: CurrencyFormatStyleConfiguration.SignDisplayStrategy { get }
```

## See Also

### Specifying sign display strategy

static var automatic: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A strategy to automatically configure sign display.

static var accounting: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to use accounting principles.

static func accountingAlways(showZero: Bool) -> CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to use accounting principles, with a configurable behavior for handling zero values.

static func always(showZero: Bool) -> CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to always show the sign, with a configurable behavior for handling zero values.

