

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.ParticleEmitter
-  ParticleEmitterComponent.ParticleEmitter.ImageSequence 

Structure

# ParticleEmitterComponent.ParticleEmitter.ImageSequence

Structure used to define properties of the sprite sheet, used by imageSequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct ImageSequence
```

## Topics

### Operators

static func == (ParticleEmitterComponent.ParticleEmitter.ImageSequence, ParticleEmitterComponent.ParticleEmitter.ImageSequence) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var animationMode: ParticleEmitterComponent.ParticleEmitter.ImageSequence.AnimationRepeatMode

How the effect timeline is played.

var columnCount: Int

Number of columns in the sprite sheet.

var frameRate: Float

Number of sprite sheet frames to play per second.

var frameRateVariation: Float

Defines a plus/minus range (in frames per second) from which a value is randomly selected to offset `frameRate`.

var hashValue: Int

The hash value.

var initialFrame: Int

First frame of the sprite sheet animation.

var initialFrameVariation: Int

Defines a plus/minus range (in frames) from which a value is randomly selected to offset `initialFrame`.

var rowCount: Int

Number of rows in the sprite sheet.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum AnimationRepeatMode

Options for how the effect timeline is played, used by the animationMode property.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable

