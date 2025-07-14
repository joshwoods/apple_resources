

- Foundation
- Decimal
- Decimal.FormatStyle
- Decimal.FormatStyle.Percent
-  notation(\_:) 

Instance Method

# notation(\_:)

Modifies the format style to use the specified notation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func notation(_ notation: Decimal.FormatStyle.Percent.Configuration.Notation) -> Decimal.FormatStyle.Percent
```

## Parameters 

`notation`  

The notation to apply to the format style.

## Return Value

A decimal percent format style modified to use the specified notation.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified decimal separator display strategy.

func grouping(Decimal.FormatStyle.Percent.Configuration.Grouping) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified grouping.

func precision(Decimal.FormatStyle.Percent.Configuration.Precision) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified precision.

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

