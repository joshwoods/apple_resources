

- Foundation
- IntegerFormatStyle
- IntegerFormatStyle.Percent
-  IntegerFormatStyle.Percent.Configuration 

Type Alias

# IntegerFormatStyle.Percent.Configuration

The type the format style uses for configuration settings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias Configuration = NumberFormatStyleConfiguration
```

## Discussion

IntegerFormatStyle.Percent uses NumberFormatStyleConfiguration for its configuration type.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: IntegerFormatStyle&lt;Value>.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified decimal separator display strategy.

func grouping(IntegerFormatStyle&lt;Value>.Percent.Configuration.Grouping) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified grouping.

func notation(IntegerFormatStyle&lt;Value>.Percent.Configuration.Notation) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified notation.

func precision(IntegerFormatStyle&lt;Value>.Percent.Configuration.Precision) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified precision.

func rounded(rule: IntegerFormatStyle&lt;Value>.Percent.Configuration.RoundingRule, increment: Int?) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified scale.

func sign(strategy: IntegerFormatStyle&lt;Value>.Percent.Configuration.SignDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified sign display strategy.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

