

- Foundation
- FloatingPointFormatStyle
- FloatingPointFormatStyle.Currency
-  grouping(\_:) 

Instance Method

# grouping(\_:)

Modifies the format style to use the specified grouping.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouping(_ group: FloatingPointFormatStyle.Currency.Configuration.Grouping) -> FloatingPointFormatStyle.Currency
```

## Parameters 

`group`  

The grouping to apply to the format style.

## Return Value

A floating-point currency format style modified to use the specified grouping.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: FloatingPointFormatStyle&lt;Value>.Currency.Configuration.DecimalSeparatorDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified decimal separator display strategy.

func precision(FloatingPointFormatStyle&lt;Value>.Currency.Configuration.Precision) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified precision.

func presentation(FloatingPointFormatStyle&lt;Value>.Currency.Configuration.Presentation) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified presentation.

func rounded(rule: FloatingPointFormatStyle&lt;Value>.Currency.Configuration.RoundingRule, increment: Double?) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified scale.

func sign(strategy: FloatingPointFormatStyle&lt;Value>.Currency.Configuration.SignDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum CurrencyFormatStyleConfiguration

Configuration settings for formatting currency values.

