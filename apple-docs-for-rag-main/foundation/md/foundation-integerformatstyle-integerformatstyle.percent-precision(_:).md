

- Foundation
- IntegerFormatStyle
- IntegerFormatStyle.Percent
-  precision(\_:) 

Instance Method

# precision(\_:)

Modifies the format style to use the specified precision.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func precision(_ p: IntegerFormatStyle.Percent.Configuration.Precision) -> IntegerFormatStyle.Percent
```

## Parameters 

`p`  

The precision to apply to the format style.

## Return Value

An integer format style modified to use the specified precision.

## Discussion

The NumberFormatStyleConfiguration.Precision type lets you specify a fixed number of digits to show for a number’s integer and fractional part, although IntegerFormatStyle.Currency only uses the former. You can also set a fixed number of significant digits.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: IntegerFormatStyle&lt;Value>.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified decimal separator display strategy.

func grouping(IntegerFormatStyle&lt;Value>.Percent.Configuration.Grouping) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified grouping.

func notation(IntegerFormatStyle&lt;Value>.Percent.Configuration.Notation) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified notation.

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

