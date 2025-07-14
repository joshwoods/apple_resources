

- RealityKit
- ParticleEmitterComponent
-  ParticleEmitterComponent.BirthDirection 

Enumeration

# ParticleEmitterComponent.BirthDirection

Options for the initial direction of each emitted particle, used by the birthDirection property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum BirthDirection
```

## Topics

### Operators

static func == (ParticleEmitterComponent.BirthDirection, ParticleEmitterComponent.BirthDirection) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case local

Emit direction is relative to the orientation of the emitter entity’s transform.

case normal

The emitting direction for each particle is along the surface normal vector at the point where the particle is emitted.

case world

Ignores the orientation from the emitter entity’s transform.

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

