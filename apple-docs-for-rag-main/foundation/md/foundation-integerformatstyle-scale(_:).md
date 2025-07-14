

- Foundation
- IntegerFormatStyle
-  scale(\_:) 

Instance Method

# scale(\_:)

Modifies the format style to use the specified scale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func scale(_ multiplicand: Double) -> IntegerFormatStyle
```

## Parameters 

`multiplicand`  

The multiplicand to apply to the format style.

## Return Value

An integer format style modified to use the specified scale.

## Discussion

The following example creates a default IntegerFormatStyle for the `en_US` locale, and a second style that scales by a multiplicand of `0.001`. It then applies each style to an array of integers. The formatting that the modified style applies expresses each value in terms of one-thousandths.

```
let defaultStyle = IntegerFormatStyle(locale: Locale(identifier: "en_US"))
let scaledStyle = defaultStyle.scale(0.001)
let nums = [100, 1000, 10000, 100000, 1000000]
let defaultNums = nums.map { defaultStyle.format($0) } // ["100", "1,000", "10,000", "100,000", "1,000,000"]
let scaledNums = nums.map { scaledStyle.format($0) } // ["0.1", "1", "10", "100", "1,000"]
```

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

func sign(strategy: IntegerFormatStyle&lt;Value>.Configuration.SignDisplayStrategy) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified sign display strategy for displaying or omitting sign symbols.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

