

- Foundation
- FloatingPointFormatStyle
- FloatingPointFormatStyle.Percent
-  scale(\_:) 

Instance Method

# scale(\_:)

Modifies the format style to use the specified scale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func scale(_ multiplicand: Double) -> FloatingPointFormatStyle.Percent
```

## Parameters 

`multiplicand`  

The multiplicand to apply to the format style.

## Return Value

A floating-point format style modified to use the specified scale.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: FloatingPointFormatStyle&lt;Value>.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified decimal separator display strategy.

func grouping(FloatingPointFormatStyle&lt;Value>.Percent.Configuration.Grouping) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified grouping.

func notation(FloatingPointFormatStyle&lt;Value>.Percent.Configuration.Notation) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified notation.

func precision(FloatingPointFormatStyle&lt;Value>.Percent.Configuration.Precision) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified precision.

func rounded(rule: FloatingPointFormatStyle&lt;Value>.Percent.Configuration.RoundingRule, increment: Double?) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified rounding rule and increment.

func sign(strategy: FloatingPointFormatStyle&lt;Value>.Percent.Configuration.SignDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

