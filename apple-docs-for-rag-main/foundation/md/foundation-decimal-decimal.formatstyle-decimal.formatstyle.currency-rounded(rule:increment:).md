

- Foundation
- Decimal
- Decimal.FormatStyle
- Decimal.FormatStyle.Currency
-  rounded(rule:increment:) 

Instance Method

# rounded(rule:increment:)

Modifies the format style to use the specified rounding rule and increment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func rounded(
    rule: Decimal.FormatStyle.Currency.Configuration.RoundingRule = .toNearestOrEven,
    increment: Int? = nil
) -> Decimal.FormatStyle.Currency
```

## Parameters 

`rule`  

The rounding rule to apply to the format style.

`increment`  

A multiple by which the formatter rounds the fractional part. The formatter produces a value that is an even multiple of this increment. If this parameter is `nil` (the default), the formatter doesn’t apply an increment.

## Return Value

A decimal currency format style modified to use the specified rounding rule and increment.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Currency.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified decimal separator display strategy.

func grouping(Decimal.FormatStyle.Currency.Configuration.Grouping) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified grouping.

func precision(Decimal.FormatStyle.Currency.Configuration.Precision) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified precision.

func presentation(Decimal.FormatStyle.Currency.Configuration.Presentation) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified presentation.

func scale(Double) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified scale.

func sign(strategy: Decimal.FormatStyle.Currency.Configuration.SignDisplayStrategy) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum CurrencyFormatStyleConfiguration

Configuration settings for formatting currency values.

