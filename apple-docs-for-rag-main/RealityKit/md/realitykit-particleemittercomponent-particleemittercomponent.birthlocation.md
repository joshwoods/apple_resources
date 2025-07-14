

- RealityKit
- ParticleEmitterComponent
-  ParticleEmitterComponent.BirthLocation 

Enumeration

# ParticleEmitterComponent.BirthLocation

Options for the location on the shape of where particles are born, used by the birthLocation property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum BirthLocation
```

## Topics

### Operators

static func == (ParticleEmitterComponent.BirthLocation, ParticleEmitterComponent.BirthLocation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case surface

Particles emit from the surface of the shape.

case vertices(count: SIMD3&lt;UInt>)

Particles emit from the vertices of the shape. `count` is the number of vertices in each direction, the distribution depends on the EmitterShape chosen.

case volume

Particles emit from the internal volume of the shape.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable

