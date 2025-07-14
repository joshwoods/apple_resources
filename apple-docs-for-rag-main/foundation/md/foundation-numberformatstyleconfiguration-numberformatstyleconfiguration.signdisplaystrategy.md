

- Foundation
- NumberFormatStyleConfiguration
-  NumberFormatStyleConfiguration.SignDisplayStrategy 

Structure

# NumberFormatStyleConfiguration.SignDisplayStrategy

A structure that an integer format style uses to configure a sign display strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SignDisplayStrategy
```

## Topics

### Sign display strategies

static var automatic: NumberFormatStyleConfiguration.SignDisplayStrategy

A strategy to automatically configure locale-appropriate sign display behavior.

static func always(includingZero: Bool) -> NumberFormatStyleConfiguration.SignDisplayStrategy

A strategy to always display sign symbols.

static var never: NumberFormatStyleConfiguration.SignDisplayStrategy

A strategy to never display sign symbols.

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

struct Notation

A structure that an integer format style uses to configure notation.

