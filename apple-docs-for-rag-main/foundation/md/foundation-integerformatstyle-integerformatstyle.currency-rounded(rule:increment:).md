

- Foundation
- IntegerFormatStyle
- IntegerFormatStyle.Currency
-  rounded(rule:increment:) 

Instance Method

# rounded(rule:increment:)

Modifies the format style to use the specified rounding rule and increment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func rounded(
    rule: IntegerFormatStyle.Currency.Configuration.RoundingRule = .toNearestOrEven,
    increment: Int? = nil
) -> IntegerFormatStyle.Currency
```

## Parameters 

`rule`  

The rounding rule to apply to the format style.

`increment`  

A multiple by which the formatter rounds the fractional part. The formatter produces a value that is an even multiple of this increment. If this parameter is `nil` (the default), the formatter doesn’t apply an increment.

## Return Value

An integer currency format style modified to use the specified rounding rule and increment.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: IntegerFormatStyle&lt;Value>.Currency.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified decimal separator display strategy.

func grouping(IntegerFormatStyle&lt;Value>.Currency.Configuration.Grouping) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified grouping.

func precision(IntegerFormatStyle&lt;Value>.Currency.Configuration.Precision) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified precision.

func presentation(IntegerFormatStyle&lt;Value>.Currency.Configuration.Presentation) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified presentation.

func scale(Double) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified scale.

func sign(strategy: IntegerFormatStyle&lt;Value>.Currency.Configuration.SignDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum CurrencyFormatStyleConfiguration

Configuration settings for formatting currency values.

