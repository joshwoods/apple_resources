

- Foundation
- FloatingPointFormatStyle
-  grouping(\_:) 

Instance Method

# grouping(\_:)

Modifies the format style to use the specified grouping.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouping(_ group: FloatingPointFormatStyle.Configuration.Grouping) -> FloatingPointFormatStyle
```

## Parameters 

`group`  

The grouping to apply to the format style.

## Return Value

A floating-point format style modified to use the specified grouping.

## Discussion

The following example creates a default FloatingPointFormatStyle for the `en_US` locale, and a second style that never uses grouping. It then applies each style to an array of floating-point values. The formatting that the the modified style applies eliminates the three-digit grouping usually performed for the `en_US` locale.

```
let defaultStyle = FloatingPointFormatStyle(locale: Locale(identifier: "en_US"))
let neverStyle = defaultStyle.grouping(.never)
let nums = [100.1, 1000.2, 10000.3, 100000.4, 1000000.5]
let defaultNums = nums.map { defaultStyle.format($0) } // ["100.1", "1,000.2", "10,000.3", "100,000.4", "1,000,000.5"]
let neverNums = nums.map { neverStyle.format($0) } // ["100.1", "1000.2", "10000.3", "100000.4", "1000000.5"]

```

## See Also

### Customizing style behavior

func decimalSeparator(strategy: FloatingPointFormatStyle&lt;Value>.Configuration.DecimalSeparatorDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified decimal separator display strategy.

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

