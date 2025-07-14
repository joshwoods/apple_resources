

- Foundation
- IntegerFormatStyle
-  IntegerFormatStyle.Configuration 

Type Alias

# IntegerFormatStyle.Configuration

The type the format style uses for configuration settings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias Configuration = NumberFormatStyleConfiguration
```

## Discussion

IntegerFormatStyle uses NumberFormatStyleConfiguration for its configuration type.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: IntegerFormatStyle&lt;Value>.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified decimal separator display strategy.

func grouping(IntegerFormatStyle&lt;Value>.Configuration.Grouping) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified grouping.

func notation(IntegerFormatStyle&lt;Value>.Configuration.Notation) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified notation.

func precision(IntegerFormatStyle&lt;Value>.Configuration.Precision) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified precision.

func rounded(rule: IntegerFormatStyle&lt;Value>.Configuration.RoundingRule, increment: Int?) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified scale.

func sign(strategy: IntegerFormatStyle&lt;Value>.Configuration.SignDisplayStrategy) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified sign display strategy for displaying or omitting sign symbols.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

