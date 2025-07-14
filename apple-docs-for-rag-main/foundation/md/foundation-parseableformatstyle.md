

- Foundation
-  ParseableFormatStyle 

Protocol

# ParseableFormatStyle

A type that can convert a given input data type into a representation in an output type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol ParseableFormatStyle : FormatStyle
```

## Topics

### Declaring Parse Strategy

var parseStrategy: Self.Strategy

**Required**

associatedtype Strategy : ParseStrategy

**Required**

### Type Properties

static var dateTime: Date.FormatStyle

static var iso8601: Date.ISO8601FormatStyle

static var number: Decimal.FormatStyle

static var percent: Decimal.FormatStyle.Percent

static var url: URL.FormatStyle

### Type Methods

static func currency(code: String) -> Self

static func name(style: PersonNameComponents.FormatStyle.Style) -> Self

## Relationships

### Inherits From

- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable

### Conforming Types

- Date.FormatStyle
- Date.ISO8601FormatStyle
- Date.VerbatimFormatStyle
- Decimal.FormatStyle
- Decimal.FormatStyle.Currency
- Decimal.FormatStyle.Percent
- FloatingPointFormatStyle

  Conforms when `Value` conforms to `BinaryFloatingPoint`.

- FloatingPointFormatStyle.Currency

  Conforms when `Value` conforms to `BinaryFloatingPoint`.

- FloatingPointFormatStyle.Percent

  Conforms when `Value` conforms to `BinaryFloatingPoint`.

- IntegerFormatStyle

  Conforms when `Value` conforms to `BinaryInteger`.

- IntegerFormatStyle.Currency

  Conforms when `Value` conforms to `BinaryInteger`.

- IntegerFormatStyle.Percent

  Conforms when `Value` conforms to `BinaryInteger`.

- PersonNameComponents.FormatStyle
- URL.FormatStyle

## See Also

### Data parsing in Swift

protocol ParseStrategy

A type that parses an input representation, such as a formatted string, into a provided data type.

struct IntegerParseStrategy

A parse strategy for creating integer values from formatted strings.

struct FloatingPointParseStrategy

A parse strategy for creating floating-point values from formatted strings.

struct ParseStrategy

A parse strategy for creating decimal values from formatted strings.

