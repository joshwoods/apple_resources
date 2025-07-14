

- Foundation
- Decimal
- Decimal.FormatStyle
- Decimal.FormatStyle.Percent
-  Decimal.FormatStyle.Percent.Configuration 

Type Alias

# Decimal.FormatStyle.Percent.Configuration

The type the format style uses for configuration settings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias Configuration = NumberFormatStyleConfiguration
```

## Discussion

Decimal.FormatStyle.Percent uses NumberFormatStyleConfiguration for its configuration type.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified decimal separator display strategy.

func grouping(Decimal.FormatStyle.Percent.Configuration.Grouping) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified grouping.

func notation(Decimal.FormatStyle.Percent.Configuration.Notation) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified notation.

func precision(Decimal.FormatStyle.Percent.Configuration.Precision) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified precision.

func rounded(rule: Decimal.FormatStyle.Percent.Configuration.RoundingRule, increment: Int?) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified scale.

func sign(strategy: Decimal.FormatStyle.Percent.Configuration.SignDisplayStrategy) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified sign display strategy.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

