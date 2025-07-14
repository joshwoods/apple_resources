

- Foundation
- CurrencyFormatStyleConfiguration
- CurrencyFormatStyleConfiguration.SignDisplayStrategy
-  automatic 

Type Property

# automatic

A strategy to automatically configure sign display.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var automatic: CurrencyFormatStyleConfiguration.SignDisplayStrategy { get }
```

## See Also

### Specifying sign display strategy

static var never: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A strategy to never show the sign.

static var accounting: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to use accounting principles.

static func accountingAlways(showZero: Bool) -> CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to use accounting principles, with a configurable behavior for handling zero values.

static func always(showZero: Bool) -> CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to always show the sign, with a configurable behavior for handling zero values.

