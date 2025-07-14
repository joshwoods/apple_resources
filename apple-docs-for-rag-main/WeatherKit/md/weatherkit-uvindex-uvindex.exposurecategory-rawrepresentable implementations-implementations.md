

- WeatherKit
- UVIndex
- UVIndex.ExposureCategory
-  RawRepresentable Implementations 

API Collection

# RawRepresentable Implementations

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `String`.

### Instance Properties

var hashValue: Int

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `String`.

func hash(into: inout Hasher)

