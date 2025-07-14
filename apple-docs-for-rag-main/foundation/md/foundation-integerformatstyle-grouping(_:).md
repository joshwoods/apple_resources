

- Foundation
- IntegerFormatStyle
-  grouping(\_:) 

Instance Method

# grouping(\_:)

Modifies the format style to use the specified grouping.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouping(_ group: IntegerFormatStyle.Configuration.Grouping) -> IntegerFormatStyle
```

## Parameters 

`group`  

The grouping to apply to the format style.

## Return Value

An integer format style modified to use the specified grouping.

## Discussion

The following example creates a default IntegerFormatStyle for the `en_US` locale, and a second style that never uses grouping. It then applies each style to an array of integers. The formatting that the modified style applies eliminates the three-digit grouping usually performed for the `en_US` locale.

```
let defaultStyle = IntegerFormatStyle(locale: Locale(identifier: "en_US"))
let neverStyle = defaultStyle.grouping(.never)
let nums = [100, 1000, 10000, 100000, 1000000]
let defaultNums = nums.map { defaultStyle.format($0) } // ["100", "1,000", "10,000", "100,000", "1,000,000"]
let neverNums = nums.map { neverStyle.format($0) } // ["100", "1000", "10000", "100000", "1000000"]
```

## See Also

### Customizing style behavior

func decimalSeparator(strategy: IntegerFormatStyle&lt;Value>.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified decimal separator display strategy.

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

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

