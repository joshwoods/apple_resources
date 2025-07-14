

- SwiftData
- Schema
- Schema.Index
-  Schema.Index.CodingKeys 

Enumeration

# Schema.Index.CodingKeys

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+Swift 5.9+

``` source
enum CodingKeys
```

## Topics

### Operators

static func == (Schema.Index&lt;T>.CodingKeys, Schema.Index&lt;T>.CodingKeys) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case indices

### Initializers

init?(intValue: Int)

Creates a new instance from the specified integer.

init?(stringValue: String)

Creates a new instance from the given string.

### Instance Properties

var hashValue: Int

The hash value.

var intValue: Int?

The value to use in an integer-indexed collection (e.g. an int-keyed dictionary).

var stringValue: String

The string to use in a named collection (e.g. a string-keyed dictionary).

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CodingKey Implementations

Equatable Implementations

## Relationships

### Conforms To

- CodingKey
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

