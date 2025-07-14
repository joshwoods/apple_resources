

- Foundation
- FloatingPointFormatStyle
- FloatingPointFormatStyle.Currency
-  sign(strategy:) 

Instance Method

# sign(strategy:)

Modifies the format style to use the specified sign display strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sign(strategy: FloatingPointFormatStyle.Currency.Configuration.SignDisplayStrategy) -> FloatingPointFormatStyle.Currency
```

## Parameters 

`strategy`  

The sign display strategy to apply to the format style.

## Return Value

A floating-point format style modified to use the specified sign display strategy.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: FloatingPointFormatStyle&lt;Value>.Currency.Configuration.DecimalSeparatorDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified decimal separator display strategy.

func grouping(FloatingPointFormatStyle&lt;Value>.Currency.Configuration.Grouping) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified grouping.

func precision(FloatingPointFormatStyle&lt;Value>.Currency.Configuration.Precision) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified precision.

func presentation(FloatingPointFormatStyle&lt;Value>.Currency.Configuration.Presentation) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified presentation.

func rounded(rule: FloatingPointFormatStyle&lt;Value>.Currency.Configuration.RoundingRule, increment: Double?) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified scale.

typealias Configuration

The type the format style uses for configuration settings.

enum CurrencyFormatStyleConfiguration

Configuration settings for formatting currency values.

