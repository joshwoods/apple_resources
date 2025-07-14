

- Foundation
- Decimal
- Decimal.FormatStyle
-  grouping(\_:) 

Instance Method

# grouping(\_:)

Modifies the format style to use the specified grouping.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouping(_ group: Decimal.FormatStyle.Configuration.Grouping) -> Decimal.FormatStyle
```

## Parameters 

`group`  

The grouping to apply to the format style.

## Return Value

A decimal format style modified to use the specified grouping.

## Discussion

The following example creates a default Decimal.FormatStyle for the `en_US` locale, and a second style that never uses grouping. It then applies each style to an array of decimal values. The formatting that the modified style applies eliminates the three-digit grouping usually performed for the `en_US` locale.

```
let defaultStyle = FloatingPointFormatStyle(locale: Locale(identifier: "en_US"))
let neverStyle = defaultStyle.grouping(.never)
let nums = [100.1, 1000.2, 10000.3, 100000.4, 1000000.5]
let defaultNums = nums.map { defaultStyle.format($0) } // ["100.1", "1,000.2", "10,000.3", "100,000.4", "1,000,000.5"]
let neverNums = nums.map { neverStyle.format($0) } // ["100.1", "1000.2", "10000.3", "100000.4", "1000000.5"]
```

## See Also

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle

Modifies the format style to use the specified decimal separator display strategy.

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

