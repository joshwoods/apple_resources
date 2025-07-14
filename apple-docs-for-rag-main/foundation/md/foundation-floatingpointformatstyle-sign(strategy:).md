

- Foundation
- FloatingPointFormatStyle
-  sign(strategy:) 

Instance Method

# sign(strategy:)

Modifies the format style to use the specified sign display strategy for displaying or omitting sign symbols.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sign(strategy: FloatingPointFormatStyle.Configuration.SignDisplayStrategy) -> FloatingPointFormatStyle
```

## Parameters 

`strategy`  

The sign display strategy to apply to the format style, such as automatic or never.

## Return Value

A floating-point format style modified to use the specified sign display strategy.

## Discussion

The following example creates a default FloatingPointFormatStyle for the `en_US` locale, and a second style that displays a sign for all values except zero. It then applies each style to an array of floating-point values. The formatting that the modified style applies adds the negative (`-`) or positive (`+`) sign to all the numbers.

```
let defaultStyle = FloatingPointFormatStyle(locale: Locale(identifier: "en_US"))
let alwaysStyle = defaultStyle.sign(strategy: .always(includingZero: false))
let nums = [-2.1, -1.2, 0, 1.4, 2.5]
let defaultNums = nums.map { defaultStyle.format($0) } // ["-2.1", "-1.2", "0", "1.4", "2.5"]
let alwaysNums = nums.map { alwaysStyle.format($0) } // ["-2.1", "-1.2", "0", "+1.4", "+2.5"]
```

## See Also

### Customizing style behavior

func decimalSeparator(strategy: FloatingPointFormatStyle&lt;Value>.Configuration.DecimalSeparatorDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified decimal separator display strategy.

func grouping(FloatingPointFormatStyle&lt;Value>.Configuration.Grouping) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified grouping.

func notation(FloatingPointFormatStyle&lt;Value>.Configuration.Notation) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified notation.

func precision(FloatingPointFormatStyle&lt;Value>.Configuration.Precision) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified precision.

func rounded(rule: FloatingPointFormatStyle&lt;Value>.Configuration.RoundingRule, increment: Double?) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified scale.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

