

- RealityKit
- ParticleEmitterComponent
-  ParticleEmitterComponent.EmitterShape 

Enumeration

# ParticleEmitterComponent.EmitterShape

Options for the shape of an emitter, used by the emitterShape property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum EmitterShape
```

## Topics

### Operators

static func == (ParticleEmitterComponent.EmitterShape, ParticleEmitterComponent.EmitterShape) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case box

Particles emit from an axis-aligned box that is centered on the origin.

case cone

Particles emit from a cone with its apex pointing up along the y-axis, centered on the origin.

case cylinder

Particles emit from a cylinder oriented vertically along the y-axis, centered on the origin.

case plane

Particles emit from a 2D plane that aligns with the x and z axes.

case point

Particles emit from a single point on the origin.

case sphere

Particles emit from a sphere centered on the origin.

case torus

Particles emit from a torus oriented along the z-axis, centered on the origin.

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

