

- Foundation
- IntegerFormatStyle
- IntegerFormatStyle.Currency
-  precision(\_:) 

Instance Method

# precision(\_:)

Modifies the format style to use the specified precision.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func precision(_ p: IntegerFormatStyle.Currency.Configuration.Precision) -> IntegerFormatStyle.Currency
```

## Parameters 

`p`  

The precision to apply to the format style.

## Return Value

An integer currency format style modified to use the specified precision.

## Discussion

The NumberFormatStyleConfiguration.Precision type lets you specify a fixed number of digits to show for a number’s integer and fractional part, although IntegerFormatStyle.Currency only uses the former. You can also set a fixed number of significant digits.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: IntegerFormatStyle&lt;Value>.Currency.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified decimal separator display strategy.

func grouping(IntegerFormatStyle&lt;Value>.Currency.Configuration.Grouping) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified grouping.

func presentation(IntegerFormatStyle&lt;Value>.Currency.Configuration.Presentation) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified presentation.

func rounded(rule: IntegerFormatStyle&lt;Value>.Currency.Configuration.RoundingRule, increment: Int?) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified scale.

func sign(strategy: IntegerFormatStyle&lt;Value>.Currency.Configuration.SignDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum CurrencyFormatStyleConfiguration

Configuration settings for formatting currency values.

