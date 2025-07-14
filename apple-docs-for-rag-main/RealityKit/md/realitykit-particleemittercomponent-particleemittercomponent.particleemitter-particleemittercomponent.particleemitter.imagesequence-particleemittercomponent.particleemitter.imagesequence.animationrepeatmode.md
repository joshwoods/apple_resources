

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.ParticleEmitter
- ParticleEmitterComponent.ParticleEmitter.ImageSequence
-  ParticleEmitterComponent.ParticleEmitter.ImageSequence.AnimationRepeatMode 

Enumeration

# ParticleEmitterComponent.ParticleEmitter.ImageSequence.AnimationRepeatMode

Options for how the effect timeline is played, used by the animationMode property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum AnimationRepeatMode
```

## Topics

### Operators

static func == (ParticleEmitterComponent.ParticleEmitter.ImageSequence.AnimationRepeatMode, ParticleEmitterComponent.ParticleEmitter.ImageSequence.AnimationRepeatMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case autoReverse

The image sequence plays through and then plays in reverse order and then repeats.

case looping

The image sequence loops repeatedly.

case playOnce

The image sequence plays once and then stops.

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

