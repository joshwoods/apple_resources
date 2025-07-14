

- SwiftData
- Schema
-  Schema.Entity 

Class

# Schema.Entity

An object that provides a blueprint for the associated model class.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
final class Entity
```

## Topics

### Creating an entity

init(String)

init(String, properties: any SchemaProperty...)

init(String, subentities: Schema.Entity..., properties: any SchemaProperty...)

### Assigning identity

var name: String

### Managing attributes

var attributes: Set&lt;Schema.Attribute>

var attributesByName: [String : Schema.Attribute]

### Defining relationships

var relationships: Set&lt;Schema.Relationship>

var relationshipsByName: [String : Schema.Relationship]

### Managing properties

var properties: [any SchemaProperty]

var inheritedProperties: [any SchemaProperty]

var inheritedPropertiesByName: [String : any SchemaProperty]

var storedProperties: [any SchemaProperty]

var storedPropertiesByName: [String : any SchemaProperty]

### Applying constraints

var uniquenessConstraints: [[String]]

### Configuring the inheritance chain

var superentity: Schema.Entity?

var superentityName: String?

var subentities: Set&lt;Schema.Entity>

### Encoding and decoding

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Comparing entities

static func == (Schema.Entity, Schema.Entity) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var debugDescription: String

A textual representation of this instance, suitable for debugging.

var hashValue: Int

The hash value.

var indices: [[String]]

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable

## See Also

### Accessing entities

let entities: [Schema.Entity]

let entitiesByName: [String : Schema.Entity]

