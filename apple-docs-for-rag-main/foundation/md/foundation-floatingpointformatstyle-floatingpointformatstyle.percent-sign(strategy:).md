

- Foundation
- FloatingPointFormatStyle
- FloatingPointFormatStyle.Percent
-  sign(strategy:) 

Instance Method

# sign(strategy:)

Modifies the format style to use the specified sign display strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sign(strategy: FloatingPointFormatStyle.Percent.Configuration.SignDisplayStrategy) -> FloatingPointFormatStyle.Percent
```

## Parameters 

`strategy`  

The sign display strategy to apply to the format style.

## Return Value

A floating-point format style modified to use the specified sign display strategy.

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

func scale(Double) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified scale.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

