

- Foundation
- Decimal
- Decimal.FormatStyle
- Decimal.FormatStyle.Percent
-  precision(\_:) 

Instance Method

# precision(\_:)

Modifies the format style to use the specified precision.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func precision(_ p: Decimal.FormatStyle.Percent.Configuration.Precision) -> Decimal.FormatStyle.Percent
```

## Parameters 

`p`  

The precision to apply to the format style.

## Return Value

A decimal format style modified to use the specified precision.

## Discussion

The NumberFormatStyleConfiguration.Precision type lets you specify a fixed number of digits to show for a number’s integer and fractional part.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified decimal separator display strategy.

func grouping(Decimal.FormatStyle.Percent.Configuration.Grouping) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified grouping.

func notation(Decimal.FormatStyle.Percent.Configuration.Notation) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified notation.

func rounded(rule: Decimal.FormatStyle.Percent.Configuration.RoundingRule, increment: Int?) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified scale.

func sign(strategy: Decimal.FormatStyle.Percent.Configuration.SignDisplayStrategy) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

