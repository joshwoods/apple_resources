

- Foundation
- IntegerFormatStyle
-  notation(\_:) 

Instance Method

# notation(\_:)

Modifies the format style to use the specified notation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func notation(_ notation: IntegerFormatStyle.Configuration.Notation) -> IntegerFormatStyle
```

## Parameters 

`notation`  

The notation to apply to the format style.

## Return Value

An integer format style modified to use the specified notation.

## Discussion

The following example creates a default IntegerFormatStyle for the `en_US` locale, and a second style that uses scientific notation style. It then applies each style to an array of integers.

```
let defaultStyle = IntegerFormatStyle(locale: Locale(identifier: "en_US"))
let scientificStyle = defaultStyle.notation(.scientific)
let nums = [100, 1000, 10000, 100000, 1000000]
let defaultNums = nums.map { defaultStyle.format($0) } // ["100", "1,000", "10,000", "100,000", "1,000,000"]
let scientificNums = nums.map { scientificStyle.format($0) } // ["1E2", "1E3", "1E4", "1E5", "1E6"]
```

## See Also

### Customizing style behavior

func decimalSeparator(strategy: IntegerFormatStyle&lt;Value>.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified decimal separator display strategy.

func grouping(IntegerFormatStyle&lt;Value>.Configuration.Grouping) -> IntegerFormatStyle&lt;Value>

Modifies the format style to use the specified grouping.

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

