

- Foundation
- Decimal
- Decimal.FormatStyle
- Decimal.FormatStyle.Currency
-  precision(\_:) 

Instance Method

# precision(\_:)

Modifies the format style to use the specified precision.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func precision(_ p: Decimal.FormatStyle.Currency.Configuration.Precision) -> Decimal.FormatStyle.Currency
```

## Parameters 

`p`  

The precision to apply to the format style.

## Return Value

A decimal format style modified to use the specified precision.

## Discussion

The NumberFormatStyleConfiguration.Precision type lets you specify a fixed number of digits to show for a number’s integer and fractional part. You can also set a fixed number of significant digits.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Currency.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified decimal separator display strategy.

func grouping(Decimal.FormatStyle.Currency.Configuration.Grouping) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified grouping.

func presentation(Decimal.FormatStyle.Currency.Configuration.Presentation) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified presentation.

func rounded(rule: Decimal.FormatStyle.Currency.Configuration.RoundingRule, increment: Int?) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified scale.

func sign(strategy: Decimal.FormatStyle.Currency.Configuration.SignDisplayStrategy) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum CurrencyFormatStyleConfiguration

Configuration settings for formatting currency values.

