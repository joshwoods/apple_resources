

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.ParticleEmitter
-  ParticleEmitterComponent.ParticleEmitter.BillboardMode 

Enumeration

# ParticleEmitterComponent.ParticleEmitter.BillboardMode

Options for specifying the axis about which the particle will be oriented, used by the `billboardMode` property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum BillboardMode
```

## Topics

### Operators

static func == (ParticleEmitterComponent.ParticleEmitter.BillboardMode, ParticleEmitterComponent.ParticleEmitter.BillboardMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case billboard

Each particle is oriented to face the camera.

case billboardYAligned

Each particle is oriented to face the camera but remains fixed about the y-axis

case free(axis: SIMD3&lt;Float>, variation: Float)

The axis about which the particle will be oriented is the given `axis`. The `variation` is a unit multiplier that determines how far from the given axis the particle is allowed to actually be oriented.

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

