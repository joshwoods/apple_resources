

- RealityKit
- ParticleEmitterComponent
-  ParticleEmitterComponent.SpawnOccasion 

Enumeration

# ParticleEmitterComponent.SpawnOccasion

Options for when the spawned effect starts, used by the spawnOccasion property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum SpawnOccasion
```

## Topics

### Operators

static func == (ParticleEmitterComponent.SpawnOccasion, ParticleEmitterComponent.SpawnOccasion) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case onBirth

The spawned effect starts at the birth time of a main particle.

case onDeath

The spawned effect starts at the death of a main particle.

case onUpdate

The spawned effect starts on every tick of the engine.

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

