

- RealityKit
- Audio
- AudioFileResource
- AudioFileResource.LoadingStrategy
-  RawRepresentable Implementations 

API Collection

# RawRepresentable Implementations

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `String`.

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var hashValue: Int

var rawValue: String

The corresponding value of the raw type.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `String`.

func hash(into: inout Hasher)

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

