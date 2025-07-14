

- Foundation
- NumberFormatStyleConfiguration
-  NumberFormatStyleConfiguration.DecimalSeparatorDisplayStrategy 

Structure

# NumberFormatStyleConfiguration.DecimalSeparatorDisplayStrategy

A structure that an integer format style uses to configure a decimal separator display strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct DecimalSeparatorDisplayStrategy
```

## Topics

### Decimal separator display strategies

static var always: NumberFormatStyleConfiguration.DecimalSeparatorDisplayStrategy

A strategy that always displays decimal separators.

static var automatic: NumberFormatStyleConfiguration.DecimalSeparatorDisplayStrategy

A strategy to automatically configure locale-appropriate decimal separator display behavior.

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Specifying Configuration

struct Grouping

A structure that an integer format style uses to configure grouping.

struct Precision

A structure that an integer format style uses to configure precision.

typealias RoundingRule

The type used for rounding rule values.

struct SignDisplayStrategy

A structure that an integer format style uses to configure a sign display strategy.

struct Notation

A structure that an integer format style uses to configure notation.

