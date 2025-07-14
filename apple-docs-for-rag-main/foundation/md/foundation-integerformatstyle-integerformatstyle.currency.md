

- Foundation
- IntegerFormatStyle
-  IntegerFormatStyle.Currency 

Structure

# IntegerFormatStyle.Currency

A format style that converts between integer currency values and their textual representations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Currency
```

Available when `Value` conforms to `BinaryInteger`.

## Topics

### Creating an integer currency format style

init(code: String, locale: Locale)

Creates an integer currency format style that uses the given currency code and locale.

### Customizing style behavior

func decimalSeparator(strategy: IntegerFormatStyle&lt;Value>.Currency.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Currency

Modifies the format style to use the specified decimal separator display strategy.

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

### Formatting integer currency values

func format(Value) -> String

Formats an integer, using this style.

### Creating attributed strings

var attributed: IntegerFormatStyle&lt;Value>.Attributed

An attributed format style based on the integer currency format style.

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

### Instance Methods

func notation(IntegerFormatStyle&lt;Value>.Currency.Configuration.Notation) -> IntegerFormatStyle&lt;Value>.Currency

### Default Implementations

FormatStyle Implementations

## Relationships

### Conforms To

- Copyable
- CustomConsumingRegexComponent
- Decodable
- Encodable
- Equatable
- FormatStyle

  Conforms when `Value` conforms to `BinaryInteger`.

- Hashable
- ParseableFormatStyle

  Conforms when `Value` conforms to `BinaryInteger`.

- RegexComponent
- Sendable

