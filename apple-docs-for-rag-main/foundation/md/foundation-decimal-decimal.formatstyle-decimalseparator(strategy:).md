

- Foundation
- Decimal
- Decimal.FormatStyle
-  decimalSeparator(strategy:) 

Instance Method

# decimalSeparator(strategy:)

Modifies the format style to use the specified decimal separator display strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func decimalSeparator(strategy: Decimal.FormatStyle.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle
```

## Parameters 

`strategy`  

The decimal separator display strategy to apply to the format style.

## Return Value

A decimal format style modified to use the specified decimal separator display strategy.

## Discussion

The following example creates a default Decimal.FormatStyle for the `en_US` locale, and a second style that uses the always strategy. It then applies each style to an array of decimal values that don’t have a fractional part. The formatting that the modified style applies adds a trailing decimal separator in all cases.

```
let defaultStyle = Decimal.FormatStyle(locale: Locale(identifier: "en_US"))
let alwaysStyle = defaultStyle.decimalSeparator(strategy: .always)
let nums: [Decimal] = [100.0, 1000.0, 10000.0, 100000.0, 1000000.0]
let defaultNums = nums.map { defaultStyle.format($0) } // ["100", "1,000", "10,000", "100,000", "1,000,000"]
let alwaysNums = nums.map { alwaysStyle.format($0) } // ["100.", "1,000.", "10,000.", "100,000.", "1,000,000."]
```

## See Also

### Customizing style behavior

func grouping(Decimal.FormatStyle.Configuration.Grouping) -> Decimal.FormatStyle

Modifies the format style to use the specified grouping.

func notation(Decimal.FormatStyle.Configuration.Notation) -> Decimal.FormatStyle

Modifies the format style to use the specified notation.

func precision(Decimal.FormatStyle.Configuration.Precision) -> Decimal.FormatStyle

Modifies the format style to use the specified precision.

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

