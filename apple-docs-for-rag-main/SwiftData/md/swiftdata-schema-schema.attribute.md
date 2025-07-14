

- SwiftData
- Schema
-  Schema.Attribute 

Class

# Schema.Attribute

An object that describes the configuration and behavior of a specific property of a model class.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
class Attribute
```

## Topics

### Creating an attribute

init(Schema.Attribute.Option..., originalName: String?, hashModifier: String?)

init(name: String, originalName: String?, options: [Schema.Attribute.Option], valueType: any Any.Type, defaultValue: Any?, hashModifier: String?)

### Specifying value information

var defaultValue: Any?

var valueType: any Any.Type

### Managing identity

var name: String

var originalName: String

### Determining behavior

var options: [Schema.Attribute.Option]

var isAttribute: Bool

var isTransformable: Bool

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

static func == (Schema.Attribute, Schema.Attribute) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Debugging

var debugDescription: String

A textual representation of this instance, suitable for debugging.

### Structures

struct Option

### Instance Properties

var hashValue: Int

The hash value.

var isOptional: Bool

var isRelationship: Bool

var isTransient: Bool

var isUnique: Bool

### Default Implementations

Equatable Implementations

## Relationships

### Inherited By

- Schema.CompositeAttribute

### Conforms To

- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- SchemaProperty

## See Also

### Attributes

class CompositeAttribute

An object that describes an attribute that derives its value by composing other attributes.

