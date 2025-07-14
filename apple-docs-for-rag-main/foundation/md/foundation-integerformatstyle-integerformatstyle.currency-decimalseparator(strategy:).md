

- Foundation
- IntegerFormatStyle
- IntegerFormatStyle.Currency
-  decimalSeparator(strategy:) 

Instance Method

# decimalSeparator(strategy:)

Modifies the format style to use the specified decimal separator display strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func decimalSeparator(strategy: IntegerFormatStyle.Currency.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle.Currency
```

## Parameters 

`strategy`  

The decimal separator display strategy to apply to the format style.

## Return Value

An integer currency format style modified to use the specified decimal separator display strategy.

## See Also

### Customizing style behavior

func grouping(IntegerFormatStyle&lt;Value>.Currency.Configuration.Grouping) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified grouping.

func precision(IntegerFormatStyle&lt;Value>.Currency.Configuration.Precision) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified precision.

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

