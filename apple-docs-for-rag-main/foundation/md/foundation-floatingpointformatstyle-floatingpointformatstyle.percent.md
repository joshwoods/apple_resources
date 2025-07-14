

- Foundation
- FloatingPointFormatStyle
-  FloatingPointFormatStyle.Percent 

Structure

# FloatingPointFormatStyle.Percent

A format style that converts between floating-point percentage values and their textual representations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Percent
```

Available when `Value` conforms to `BinaryFloatingPoint`.

## Topics

### Creating a floating-point percent format style

init(locale: Locale)

Creates a floating-point percent format style that uses the given locale.

### Customizing style behavior

func decimalSeparator(strategy: FloatingPointFormatStyle&lt;Value>.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified decimal separator display strategy.

func grouping(FloatingPointFormatStyle&lt;Value>.Percent.Configuration.Grouping) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified grouping.

func notation(FloatingPointFormatStyle&lt;Value>.Percent.Configuration.Notation) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified notation.

func precision(FloatingPointFormatStyle&lt;Value>.Percent.Configuration.Precision) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified precision.

func rounded(rule: FloatingPointFormatStyle&lt;Value>.Percent.Configuration.RoundingRule, increment: Double?) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified scale.

func sign(strategy: FloatingPointFormatStyle&lt;Value>.Percent.Configuration.SignDisplayStrategy) -> FloatingPointFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

### Creating attributed strings

var attributed: FloatingPointFormatStyle&lt;Value>.Attributed

An attributed format style based on the floating-point percent format style.

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

  Conforms when `Value` conforms to `BinaryFloatingPoint`.

- Hashable
- ParseableFormatStyle

  Conforms when `Value` conforms to `BinaryFloatingPoint`.

- RegexComponent
- Sendable

## See Also

### Supporting types

struct Currency

A format style that converts between floating-point currency values and their textual representations.

