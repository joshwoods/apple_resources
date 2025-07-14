

- Foundation
- Decimal
- Decimal.FormatStyle
-  Decimal.FormatStyle.Percent 

Structure

# Decimal.FormatStyle.Percent

A format style that converts between decimal percentage values and their textual representations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Percent
```

## Topics

### Creating a decimal percent format style

init(locale: Locale)

Creates a decimal percent format style that uses the given locale.

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified decimal separator display strategy.

func grouping(Decimal.FormatStyle.Percent.Configuration.Grouping) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified grouping.

func notation(Decimal.FormatStyle.Percent.Configuration.Notation) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified notation.

func precision(Decimal.FormatStyle.Percent.Configuration.Precision) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified precision.

func rounded(rule: Decimal.FormatStyle.Percent.Configuration.RoundingRule, increment: Int?) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified scale.

func sign(strategy: Decimal.FormatStyle.Percent.Configuration.SignDisplayStrategy) -> Decimal.FormatStyle.Percent

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

### Creating attributed strings

var attributed: Decimal.FormatStyle.Attributed

An attributed format style based on the decimal percent format style.

struct Attributed

A format style that converts integers into attributed strings.

### Accessing style properties

var locale: Locale

The locale of the format style.

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

## See Also

### Supporting types

struct Currency

A format style that converts between decimal currency values and their textual representations.

