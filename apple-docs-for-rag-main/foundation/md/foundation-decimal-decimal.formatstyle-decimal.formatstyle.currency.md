

- Foundation
- Decimal
- Decimal.FormatStyle
-  Decimal.FormatStyle.Currency 

Structure

# Decimal.FormatStyle.Currency

A format style that converts between decimal currency values and their textual representations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Currency
```

## Topics

### Creating a decimal currency style

init(code: String, locale: Locale)

Creates a decimal currency format style that uses the given currency code and locale.

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Currency.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified decimal separator display strategy.

func grouping(Decimal.FormatStyle.Currency.Configuration.Grouping) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified grouping.

func precision(Decimal.FormatStyle.Currency.Configuration.Precision) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified precision.

func presentation(Decimal.FormatStyle.Currency.Configuration.Presentation) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified presentation.

func rounded(rule: Decimal.FormatStyle.Currency.Configuration.RoundingRule, increment: Int?) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified scale.

func sign(strategy: Decimal.FormatStyle.Currency.Configuration.SignDisplayStrategy) -> Decimal.FormatStyle.Currency

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum CurrencyFormatStyleConfiguration

Configuration settings for formatting currency values.

### Creating attributed strings

var attributed: Decimal.FormatStyle.Attributed

An attributed format style based on the decimal currency format style.

struct Attributed

A format style that converts integers into attributed strings.

### Accessing style properties

var currencyCode: String

The currency code this format style uses.

var locale: Locale

The locale of the format style.

### Instance Methods

func notation(Decimal.FormatStyle.Currency.Configuration.Notation) -> Decimal.FormatStyle.Currency

## Relationships

### Conforms To

- Copyable
- CustomConsumingRegexComponent
- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable
- ParseableFormatStyle
- RegexComponent
- Sendable

