

- Foundation
- FloatingPointFormatStyle
-  precision(\_:) 

Instance Method

# precision(\_:)

Modifies the format style to use the specified precision.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func precision(_ p: FloatingPointFormatStyle.Configuration.Precision) -> FloatingPointFormatStyle
```

## Parameters 

`p`  

The precision to apply to the format style.

## Return Value

A floating-point format style modified to use the specified precision.

## Discussion

The NumberFormatStyleConfiguration.Precision type lets you specify a fixed number of digits to show for a number’s integer and fractional parts. You can also set a fixed number of significant digits.

The following example creates a default FloatingPointFormatStyle for the `en_US` locale, and a second style that uses a maximum of four significant digits. It then applies each style to an array of floating-point values. The formatting that the modified style applies truncates precision to `0` after the fourth most-significant digit.

```
let defaultStyle = FloatingPointFormatStyle(locale: Locale(identifier: "en_US"))
let precisionStyle = defaultStyle.precision(.significantDigits(1...4))
let nums = [123.1, 1234.1, 12345.1, 123456.1, 1234567.1]
let defaultNums = nums.map { defaultStyle.format($0) } // ["123.1", "1,234.1", "12,345.1", "123,456.1", "1,234,567.1"]
let precisionNums = nums.map { precisionStyle.format($0) } // ["123.1", "1,234", "12,350", "123,500", "1,235,000"]
```

## See Also

### Customizing style behavior

func decimalSeparator(strategy: FloatingPointFormatStyle&lt;Value>.Configuration.DecimalSeparatorDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified decimal separator display strategy.

func grouping(FloatingPointFormatStyle&lt;Value>.Configuration.Grouping) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified grouping.

func notation(FloatingPointFormatStyle&lt;Value>.Configuration.Notation) -> FloatingPointFormatStyle&lt;Value>

Modifies the format style to use the specified notation.

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

