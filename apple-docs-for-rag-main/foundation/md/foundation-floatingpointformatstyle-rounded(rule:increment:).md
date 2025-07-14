

- Foundation
- FloatingPointFormatStyle
-  rounded(rule:increment:) 

Instance Method

# rounded(rule:increment:)

Modifies the format style to use the specified rounding rule and increment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func rounded(
    rule: FloatingPointFormatStyle.Configuration.RoundingRule = .toNearestOrEven,
    increment: Double? = nil
) -> FloatingPointFormatStyle
```

## Parameters 

`rule`  

The rounding rule to apply to the format style.

`increment`  

A multiple by which the formatter rounds the fractional part. The formatter produces a value that is an even multiple of this increment. If this parameter is `nil` (the default), the formatter doesn’t apply an increment.

## Return Value

A floating-point format style modified to use the specified rounding rule and increment.

## Discussion

The following example creates a default FloatingPointFormatStyle for the `en_US` locale, and modifies its rounding behavior. It uses the FloatingPointRoundingRule.up rounding rule, and an increment of `0.25`. It then applies this style to an array of floating-point values, rounding them to the next greater increment of 0.25.

```
let roundedStyle = FloatingPointFormatStyle(locale: Locale(identifier: "en_US"))
    .rounded(rule: .up, increment: 0.25)
let nums = [1.0, 1.1, 1.2, 1.3, 1.4, 1.5, 1.6]
let roundedNums = nums.map { roundedStyle.format($0) } // ["1.00", "1.25", "1.25", "1.50", "1.50", "1.50", "1.75"]
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

func scale(Double) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified scale.

func sign(strategy: FloatingPointFormatStyle&lt;Value>.Configuration.SignDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified sign display strategy for displaying or omitting sign symbols.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

