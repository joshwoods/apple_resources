

- Foundation
- Decimal
- Decimal.FormatStyle
-  precision(\_:) 

Instance Method

# precision(\_:)

Modifies the format style to use the specified precision.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func precision(_ p: Decimal.FormatStyle.Configuration.Precision) -> Decimal.FormatStyle
```

## Parameters 

`p`  

The precision to apply to the format style.

## Return Value

A decimal format style modified to use the specified precision.

## Discussion

The NumberFormatStyleConfiguration.Precision type lets you specify fixed numbers of digits to show for a number’s integer and fractional parts. You can also set a fixed number of significant digits.

The following example creates a default Decimal.FormatStyle for the `en_US` locale, and a second style that uses a maximum of four significant digits. It then applies each style to an array of decimal values. The formatting applied by the modified style truncates precision to `0` after the fourth most-significant digit.

```
let defaultStyle = Decimal.FormatStyle(locale: Locale(identifier: "en_US"))
let precisionStyle = defaultStyle.precision(.significantDigits(1...4))
let nums: [Decimal] = [123.1, 1234.1, 12345.1, 123456.1, 1234567.1]
let defaultNums = nums.map { defaultStyle.format($0) } // ["123.1", "1,234.1", "12,345.1", "123,456.1", "1,234,567.1"]
let precisionNums = nums.map { precisionStyle.format($0) } // ["123.1", "1,234", "12,350", "123,500", "1,235,000"]
```

## See Also

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle

Modifies the format style to use the specified decimal separator display strategy.

func grouping(Decimal.FormatStyle.Configuration.Grouping) -> Decimal.FormatStyle

Modifies the format style to use the specified grouping.

func notation(Decimal.FormatStyle.Configuration.Notation) -> Decimal.FormatStyle

Modifies the format style to use the specified notation.

func rounded(rule: Decimal.FormatStyle.Configuration.RoundingRule, increment: Int?) -> Decimal.FormatStyle

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> Decimal.FormatStyle

Modifies the format style to use the specified scale.

func sign(strategy: Decimal.FormatStyle.Configuration.SignDisplayStrategy) -> Decimal.FormatStyle

Modifies the format style to use the specified sign display strategy for displaying or omitting sign symbols.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

