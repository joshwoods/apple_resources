

- SwiftData
- Schema
-  Schema.Relationship 

Class

# Schema.Relationship

An object that describes the configuration and behavior of a relationship between two model classes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
final class Relationship
```

## Topics

### Creating a relationship

init(Schema.Relationship.Option..., deleteRule: Schema.Relationship.DeleteRule, minimumModelCount: Int?, maximumModelCount: Int?, originalName: String?, inverse: AnyKeyPath?, hashModifier: String?)

### Managing the configuration

var keypath: AnyKeyPath?

var destination: String

var inverseName: String?

var inverseKeyPath: AnyKeyPath?

var deleteRule: Schema.Relationship.DeleteRule

enum DeleteRule

Describes the rule to apply when deleting a model containing references to other models.

var isToOneRelationship: Bool

### Specifying value information

var valueType: any Any.Type

### Managing identity

var name: String

var originalName: String

### Determining behavior

var options: [Schema.Relationship.Option]

### Versioning

var hashModifier: String?

### Encoding and decoding

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Comparing attributes

static func == (Schema.Relationship, Schema.Relationship) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Debugging

var debugDescription: String

A textual representation of this instance, suitable for debugging.

### Structures

struct Option

### Instance Properties

var hashValue: Int

The hash value.

var isAttribute: Bool

var isTransient: Bool

var isUnique: Bool

var maximumModelCount: Int?

var minimumModelCount: Int?

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

