

- Foundation
- CurrencyFormatStyleConfiguration
- CurrencyFormatStyleConfiguration.SignDisplayStrategy
-  accountingAlways(showZero:) 

Type Method

# accountingAlways(showZero:)

A sign display strategy to use accounting principles, with a configurable behavior for handling zero values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func accountingAlways(showZero: Bool = false) -> CurrencyFormatStyleConfiguration.SignDisplayStrategy
```

## Parameters 

`showZero`  

A Boolean value that indicates whether to show the sign symbol on zero values. Defaults to `false`.

## Return Value

A strategy that uses accounting principles, and the specified handling of zero values.

## See Also

### Specifying sign display strategy

static var never: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A strategy to never show the sign.

static var automatic: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A strategy to automatically configure sign display.

static var accounting: CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to use accounting principles.

static func always(showZero: Bool) -> CurrencyFormatStyleConfiguration.SignDisplayStrategy

A sign display strategy to always show the sign, with a configurable behavior for handling zero values.

