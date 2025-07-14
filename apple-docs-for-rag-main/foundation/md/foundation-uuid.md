

- Foundation
-  UUID 

Structure

# UUID

A universally unique value to identify types, interfaces, and other items.

iOS 6.0+iPadOS 6.0+Mac Catalyst 6.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct UUID
```

## Topics

### Creating UUIDs

init()

Creates a UUID with RFC 4122 version 4 random bytes.

init(uuid: uuid_t)

Creates a UUID from the uuid C-language structure.

init?(uuidString: String)

Creates a UUID from a string representation.

### Getting UUID Values

var uuid: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

Returns the UUID as bytes.

var uuidString: String

Returns a string created from the UUID, such as “E621E1F8-C36C-495A-93FC-0C247A3E6E5F”

### Comparing UUIDs

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Using Reference Types

class NSUUID

A universally unique value that can be used to identify types, interfaces, and other items.

### Default Implementations

EntityIdentifierConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- EntityIdentifierConvertible
- Equatable
- Hashable
- ReferenceConvertible
- Sendable

