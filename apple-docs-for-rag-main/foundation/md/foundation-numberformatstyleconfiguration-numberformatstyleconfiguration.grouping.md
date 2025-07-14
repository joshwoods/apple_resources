

- Foundation
- NumberFormatStyleConfiguration
-  NumberFormatStyleConfiguration.Grouping 

Structure

# NumberFormatStyleConfiguration.Grouping

A structure that an integer format style uses to configure grouping.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Grouping
```

## Topics

### Grouping configurations

static var automatic: NumberFormatStyleConfiguration.Grouping

A grouping behvaior that automatically applies locale-appropriate grouping.

static var never: NumberFormatStyleConfiguration.Grouping

A grouping behvaior that never groups digits.

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

struct Precision

A structure that an integer format style uses to configure precision.

typealias RoundingRule

The type used for rounding rule values.

struct SignDisplayStrategy

A structure that an integer format style uses to configure a sign display strategy.

struct Notation

A structure that an integer format style uses to configure notation.

