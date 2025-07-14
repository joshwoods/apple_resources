

- Foundation
- Decimal
- Decimal.FormatStyle
-  scale(\_:) 

Instance Method

# scale(\_:)

Modifies the format style to use the specified scale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func scale(_ multiplicand: Double) -> Decimal.FormatStyle
```

## Parameters 

`multiplicand`  

The multiplicand to apply to the format style.

## Return Value

A decimal format style modified to use the specified scale.

## Discussion

The following example creates a default Decimal.FormatStyle for the `en_US` locale, and a second style that scales by a `multiplicand` of `0.001`. It then applies each style to an array of decimal values. The formatting that the modified style applies expresses each value in terms of one-thousandths.

```
let defaultStyle = Decimal.FormatStyle(locale: Locale(identifier: "en_US"))
let scaledStyle = defaultStyle.scale(0.001)
let nums: [Decimal] = [100.1, 1000.2, 10000.3, 100000.4, 1000000.5]
let defaultNums = nums.map { defaultStyle.format($0) } // ["100.1", "1,000.2", "10,000.3", "100,000.4", "1,000,000.5"]
let scaledNums = nums.map { scaledStyle.format($0) } // ["0.1001", "1.0002", "10.0003", "100.0004", "1,000.0005"]
```

## See Also

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle

Modifies the format style to use the specified decimal separator display strategy.

func grouping(Decimal.FormatStyle.Configuration.Grouping) -> Decimal.FormatStyle

Modifies the format style to use the specified grouping.

func notation(Decimal.FormatStyle.Configuration.Notation) -> Decimal.FormatStyle

Modifies the format style to use the specified notation.

func precision(Decimal.FormatStyle.Configuration.Precision) -> Decimal.FormatStyle

Modifies the format style to use the specified precision.

func rounded(rule: Decimal.FormatStyle.Configuration.RoundingRule, increment: Int?) -> Decimal.FormatStyle

Modifies the format style to use the specified rounding rule and increment.

func sign(strategy: Decimal.FormatStyle.Configuration.SignDisplayStrategy) -> Decimal.FormatStyle

Modifies the format style to use the specified sign display strategy for displaying or omitting sign symbols.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

