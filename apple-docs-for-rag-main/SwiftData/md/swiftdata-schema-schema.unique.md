

- SwiftData
- Schema
-  Schema.Unique 

Class

# Schema.Unique

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+Swift 5.9+

``` source
final class Unique where T : PersistentModel
```

## Topics

### Operators

static func == (Schema.Unique&lt;T>, Schema.Unique&lt;T>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init([PartialKeyPath&lt;T>]...)

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

let constraints: [[PartialKeyPath&lt;T>]]

var debugDescription: String

A textual representation of this instance, suitable for debugging.

var hashValue: Int

The hash value.

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

