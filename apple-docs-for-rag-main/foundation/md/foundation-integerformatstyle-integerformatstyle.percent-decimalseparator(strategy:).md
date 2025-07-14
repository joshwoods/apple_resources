

- Foundation
- IntegerFormatStyle
- IntegerFormatStyle.Percent
-  decimalSeparator(strategy:) 

Instance Method

# decimalSeparator(strategy:)

Modifies the format style to use the specified decimal separator display strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func decimalSeparator(strategy: IntegerFormatStyle.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle.Percent
```

## Parameters 

`strategy`  

The decimal separator display strategy to apply to the format style.

## Return Value

An integer percent format style modified to use the specified decimal separator display strategy.

## See Also

### Customizing style behavior

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

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

