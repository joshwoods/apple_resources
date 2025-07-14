

- Foundation
- FloatingPointFormatStyle
-  decimalSeparator(strategy:) 

Instance Method

# decimalSeparator(strategy:)

Modifies the format style to use the specified decimal separator display strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func decimalSeparator(strategy: FloatingPointFormatStyle.Configuration.DecimalSeparatorDisplayStrategy) -> FloatingPointFormatStyle
```

## Parameters 

`strategy`  

The decimal separator display strategy to apply to the format style.

## Return Value

A floating-point format style modified to use the specified decimal separator display strategy.

## Discussion

The following example creates a default FloatingPointFormatStyle for the `en_US` locale, and a second style that uses the always strategy. It then applies each style to an array of floating-point values that don’t have a fractional part. The formatting that the modified style applies adds a trailing decimal separator in all cases.

```
let defaultStyle = FloatingPointFormatStyle(locale: Locale(identifier: "en_US"))
let alwaysStyle = defaultStyle.decimalSeparator(strategy: .always)
let nums = [100.0, 1000.0, 10000.0, 100000.0, 1000000.0]
let defaultNums = nums.map { defaultStyle.format($0) } // ["100", "1,000", "10,000", "100,000", "1,000,000"]
let alwaysNums = nums.map { alwaysStyle.format($0) } // ["100.", "1,000.", "10,000.", "100,000.", "1,000,000."]

```

## See Also

### Customizing style behavior

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

func sign(strategy: FloatingPointFormatStyle&lt;Value>.Configuration.SignDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified sign display strategy for displaying or omitting sign symbols.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

