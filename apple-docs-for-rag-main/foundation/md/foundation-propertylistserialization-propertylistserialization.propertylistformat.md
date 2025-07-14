

- Foundation
- PropertyListSerialization
-  PropertyListSerialization.PropertyListFormat 

Enumeration

# PropertyListSerialization.PropertyListFormat

These constants are used to specify a property list serialization format.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum PropertyListFormat
```

## Topics

### Constants

case openStep

Specifies the ASCII property list format inherited from the OpenStep APIs.

case xml

Specifies the XML property list format.

case binary

Specifies the binary property list format.

case openStep

Specifies the ASCII property list format inherited from the OpenStep APIs.

case xml

Specifies the XML property list format.

case binary

Specifies the binary property list format.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct MutabilityOptions

These constants specify mutability options in property lists.

typealias ReadOptions

The only read options supported are described in PropertyListSerialization.MutabilityOptions.

