

- SwiftData
- Schema
-  Schema.Index 

Class

# Schema.Index

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+Swift 5.9+

``` source
final class Index where T : PersistentModel
```

## Topics

### Operators

static func == (Schema.Index&lt;T>, Schema.Index&lt;T>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(Schema.Index&lt;T>.Types&lt;T>...)

init([PartialKeyPath&lt;T>]...)

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var debugDescription: String

A textual representation of this instance, suitable for debugging.

var hashValue: Int

The hash value.

let indices: [Schema.Index&lt;T>.Types&lt;T>]

var isUnique: Bool

var name: String

var originalName: String

var valueType: any Any.Type

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum CodingKeys

enum Types

### Default Implementations

Equatable Implementations

SchemaProperty Implementations

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- SchemaProperty

