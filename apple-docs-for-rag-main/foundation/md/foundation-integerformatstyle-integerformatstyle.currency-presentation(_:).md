

- Foundation
- IntegerFormatStyle
- IntegerFormatStyle.Currency
-  presentation(\_:) 

Instance Method

# presentation(\_:)

Modifies the format style to use the specified presentation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func presentation(_ p: IntegerFormatStyle.Currency.Configuration.Presentation) -> IntegerFormatStyle.Currency
```

## Parameters 

`p`  

A currency presentation value, such as isoCode or fullName.

## Return Value

An integer currency format style modified to use the specified presentation.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: IntegerFormatStyle&lt;Value>.Currency.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified decimal separator display strategy.

func grouping(IntegerFormatStyle&lt;Value>.Currency.Configuration.Grouping) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified grouping.

func precision(IntegerFormatStyle&lt;Value>.Currency.Configuration.Precision) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified precision.

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

