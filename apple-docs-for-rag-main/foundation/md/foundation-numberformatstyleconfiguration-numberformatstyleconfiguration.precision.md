

- Foundation
- NumberFormatStyleConfiguration
-  NumberFormatStyleConfiguration.Precision 

Structure

# NumberFormatStyleConfiguration.Precision

A structure that an integer format style uses to configure precision.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Precision
```

## Topics

### Precision configurations

static func significantDigits&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of significant digits.

static func significantDigits(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of significant digits.

static func integerAndFractionLength&lt;R1, R2>(integerLimits: R1, fractionLimits: R2) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to ranges of allowed digits in the integer and fraction parts.

static func integerAndFractionLength(integer: Int, fraction: Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values a given number of allowed digits in the integer and fraction parts.

static func integerLength&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of allowed digits in the integer part.

static func integerLength(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of allowed digits in the integer part.

static func fractionLength&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of allowed digits in the fraction part.

static func fractionLength(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of allowed digits in the fraction part.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Specifying Configuration

struct DecimalSeparatorDisplayStrategy

A structure that an integer format style uses to configure a decimal separator display strategy.

struct Grouping

A structure that an integer format style uses to configure grouping.

typealias RoundingRule

The type used for rounding rule values.

struct SignDisplayStrategy

A structure that an integer format style uses to configure a sign display strategy.

struct Notation

A structure that an integer format style uses to configure notation.

