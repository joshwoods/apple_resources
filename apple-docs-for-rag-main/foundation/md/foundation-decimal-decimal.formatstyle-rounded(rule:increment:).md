

- Foundation
- Decimal
- Decimal.FormatStyle
-  rounded(rule:increment:) 

Instance Method

# rounded(rule:increment:)

Modifies the format style to use the specified rounding rule and increment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func rounded(
    rule: Decimal.FormatStyle.Configuration.RoundingRule = .toNearestOrEven,
    increment: Int? = nil
) -> Decimal.FormatStyle
```

## Parameters 

`rule`  

The rounding rule to apply to the format style.

`increment`  

A multiple by which the formatter rounds the fractional part. The formatter produces a value that is an even multiple of this increment. If this parameter is `nil` (the default), the formatter doesn’t apply an increment.

## Return Value

A decimal format style modified to use the specified rounding rule and increment.

## Discussion

The following example creates a default Decimal.FormatStyle for the `en_US` locale, and a modified style that rounds integers to the nearest multiple of `100`. It then formats the value `1999.95` using these format styles.

```
let defaultStyle = Decimal.FormatStyle(locale: Locale(identifier: "en_US"))
let roundedStyle = defaultStyle.rounded(rule: .toNearestOrEven,
                                        increment: 100)
let num: Decimal = 1999.95
let defaultNum = num.formatted(defaultStyle) // "1,999.95"
let roundedNum = num.formatted(roundedStyle) // "2,000"
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

func scale(Double) -> Decimal.FormatStyle

Modifies the format style to use the specified scale.

func sign(strategy: Decimal.FormatStyle.Configuration.SignDisplayStrategy) -> Decimal.FormatStyle

Modifies the format style to use the specified sign display strategy for displaying or omitting sign symbols.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

