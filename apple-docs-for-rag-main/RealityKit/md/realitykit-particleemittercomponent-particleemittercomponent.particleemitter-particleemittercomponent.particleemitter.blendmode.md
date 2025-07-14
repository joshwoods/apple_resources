

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.ParticleEmitter
-  ParticleEmitterComponent.ParticleEmitter.BlendMode 

Enumeration

# ParticleEmitterComponent.ParticleEmitter.BlendMode

Options for combining source and destination pixel colors when compositing particles during rendering, used by the blendMode property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum BlendMode
```

## Topics

### Operators

static func == (ParticleEmitterComponent.ParticleEmitter.BlendMode, ParticleEmitterComponent.ParticleEmitter.BlendMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case additive

The source and destination colors are added together.

case alpha

The source and destination colors are blended by multiplying the source alpha value.

case opaque

The particle fully occludes anything drawn before it.

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

