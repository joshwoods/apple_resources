

- Foundation
- NumberFormatStyleConfiguration
-  NumberFormatStyleConfiguration.Notation 

Structure

# NumberFormatStyleConfiguration.Notation

A structure that an integer format style uses to configure notation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Notation
```

## Topics

### Notations

static var automatic: NumberFormatStyleConfiguration.Notation

A notation that automatically provides locale-appropriate behavior.

static var compactName: NumberFormatStyleConfiguration.Notation

A locale-appropriate compact name notation.

static var scientific: NumberFormatStyleConfiguration.Notation

A notation constant that formats values with scientific notation.

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

struct DecimalSeparatorDisplayStrategy

A structure that an integer format style uses to configure a decimal separator display strategy.

struct Grouping

A structure that an integer format style uses to configure grouping.

struct Precision

A structure that an integer format style uses to configure precision.

typealias RoundingRule

The type used for rounding rule values.

struct SignDisplayStrategy

A structure that an integer format style uses to configure a sign display strategy.

