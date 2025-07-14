

- Foundation
- FloatingPointFormatStyle
-  FloatingPointFormatStyle.Currency 

Structure

# FloatingPointFormatStyle.Currency

A format style that converts between floating-point currency values and their textual representations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Currency
```

Available when `Value` conforms to `BinaryFloatingPoint`.

## Topics

### Creating a floating-point currency style

init(code: String, locale: Locale)

Creates a floating-point currency format style that uses the given currency code and locale.

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

func sign(strategy: FloatingPointFormatStyle&lt;Value>.Currency.Configuration.SignDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum CurrencyFormatStyleConfiguration

Configuration settings for formatting currency values.

### Creating attributed strings

var attributed: FloatingPointFormatStyle&lt;Value>.Attributed

An attributed format style based on the floating-point currency format style.

struct Attributed

A format style that converts integers into attributed strings.

### Accessing style properties

let currencyCode: String

The currency code this format style uses.

var locale: Locale

The locale of the format style.

### Applying measurement styles

struct FormatStyle

A type that provides localized representations of measurements.

### Applying list styles

struct ListFormatStyle

A type that formats lists of items with a separator and conjunction appropriate for a given locale.

### Instance Methods

func notation(FloatingPointFormatStyle&lt;Value>.Currency.Configuration.Notation) -> FloatingPointFormatStyle&lt;Value>.Currency

## Relationships

### Conforms To

- Copyable
- CustomConsumingRegexComponent
- Decodable
- Encodable
- Equatable
- FormatStyle

  Conforms when `Value` conforms to `BinaryFloatingPoint`.

- Hashable
- ParseableFormatStyle

  Conforms when `Value` conforms to `BinaryFloatingPoint`.

- RegexComponent
- Sendable

