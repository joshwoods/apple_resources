

- Foundation
- FloatingPointFormatStyle
- FloatingPointFormatStyle.Percent
-  decimalSeparator(strategy:) 

Instance Method

# decimalSeparator(strategy:)

Modifies the format style to use the specified decimal separator display strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func decimalSeparator(strategy: FloatingPointFormatStyle.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> FloatingPointFormatStyle.Percent
```

## Parameters 

`strategy`  

The decimal separator display strategy to apply to the format style.

## Return Value

A floating-point percent format style modified to use the specified decimal separator display strategy.

## See Also

### Customizing style behavior

func grouping(FloatingPointFormatStyle&lt;Value>.Percent.Configuration.Grouping) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified grouping.

func notation(FloatingPointFormatStyle&lt;Value>.Percent.Configuration.Notation) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified notation.

func precision(FloatingPointFormatStyle&lt;Value>.Percent.Configuration.Precision) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified precision.

func rounded(rule: FloatingPointFormatStyle&lt;Value>.Percent.Configuration.RoundingRule, increment: Double?) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified scale.

func sign(strategy: FloatingPointFormatStyle&lt;Value>.Percent.Configuration.SignDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

