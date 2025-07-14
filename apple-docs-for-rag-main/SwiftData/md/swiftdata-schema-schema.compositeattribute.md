

- SwiftData
- Schema
-  Schema.CompositeAttribute 

Class

# Schema.CompositeAttribute

An object that describes an attribute that derives its value by composing other attributes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
final class CompositeAttribute
```

## Topics

### Creating a composite attribute

init(name: String, originalName: String?, options: [Schema.Attribute.Option], valueType: any Any.Type, defaultValue: Any?, hashModifier: String?)

### Composing attributes

var properties: [Schema.Attribute]

### Encoding and decoding

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

init(from: any Decoder) throws

### Debugging

var debugDescription: String

A textual representation of this instance, suitable for debugging.

## Relationships

### Inherits From

- Schema.Attribute

### Conforms To

- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- SchemaProperty

## See Also

### Attributes

class Attribute

An object that describes the configuration and behavior of a specific property of a model class.

