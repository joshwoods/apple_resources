

- Foundation
- IntegerFormatStyle
-  IntegerFormatStyle.Percent 

Structure

# IntegerFormatStyle.Percent

A format style that converts between integer percentage values and their textual representations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Percent
```

Available when `Value` conforms to `BinaryInteger`.

## Topics

### Creating an integer percent format style

init(locale: Locale)

Creates an integer percent format style that uses the given locale.

### Customizing style behavior

func decimalSeparator(strategy: IntegerFormatStyle&lt;Value>.Percent.Configuration.DecimalSeparatorDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified decimal separator display strategy.

func grouping(IntegerFormatStyle&lt;Value>.Percent.Configuration.Grouping) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified grouping.

func notation(IntegerFormatStyle&lt;Value>.Percent.Configuration.Notation) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified notation.

func precision(IntegerFormatStyle&lt;Value>.Percent.Configuration.Precision) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified precision.

func rounded(rule: IntegerFormatStyle&lt;Value>.Percent.Configuration.RoundingRule, increment: Int?) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified scale.

func sign(strategy: IntegerFormatStyle&lt;Value>.Percent.Configuration.SignDisplayStrategy) -> IntegerFormatStyle&lt;Value>.Percent

Modifies the format style to use the specified sign display strategy.

typealias Configuration

The type the format style uses for configuration settings.

enum NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

### Formatting integer percent values

func format(Value) -> String

Formats an integer, using this style.

### Creating attributed strings

var attributed: IntegerFormatStyle&lt;Value>.Attributed

An attributed format style based on the integer percent format style.

struct Attributed

A format style that converts integers into attributed strings.

### Accessing style properties

var locale: Locale

The locale of the format style.

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

## See Also

### Applying percentage styles for integers

static var percent: IntegerFormatStyle&lt;Int>.Percent

A style for formatting signed integer types in Swift as a percent representation.

static var percent: IntegerFormatStyle&lt;UInt>.Percent

A style for formatting signed integer types in Swift as a percent representation.

static var percent: IntegerFormatStyle&lt;Int8>.Percent

A style for formatting 8-bit signed integers as a percent representation.

static var percent: IntegerFormatStyle&lt;Int16>.Percent

A style for formatting 16-bit signed integers as a percent representation.

static var percent: IntegerFormatStyle&lt;Int32>.Percent

A style for formatting 32-bit signed integers as a percent representation.

static var percent: IntegerFormatStyle&lt;Int64>.Percent

A style for formatting 64-bit signed integers as a percent representation.

static var percent: IntegerFormatStyle&lt;UInt8>.Percent

A style for formatting 8-bit unsigned integers as a percent representation.

static var percent: IntegerFormatStyle&lt;UInt16>.Percent

A style for formatting 16-bit unsigned integers as a percent representation.

static var percent: IntegerFormatStyle&lt;UInt32>.Percent

A style for formatting 32-bit unsigned integers as a percent representation.

static var percent: IntegerFormatStyle&lt;UInt64>.Percent

A style for formatting 64-bit unsigned integers as a percent representation.

