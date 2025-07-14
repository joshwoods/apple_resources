

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.ParticleEmitter
-  ParticleEmitterComponent.ParticleEmitter.SortOrder 

Enumeration

# ParticleEmitterComponent.ParticleEmitter.SortOrder

Options for the rendering order of particles, used by the sortingMode property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum SortOrder
```

## Topics

### Operators

static func == (ParticleEmitterComponent.ParticleEmitter.SortOrder, ParticleEmitterComponent.ParticleEmitter.SortOrder) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case decreasingAge

Particles emitted earlier are rendered before particles emitted more recently.

case decreasingDepth

Particles closer to camera are rendered first

case decreasingID

Particles with higher IDs are rendered first

case increasingAge

Particles emitted more recently are rendered before particles emitted earlier.

case increasingDepth

Particles further from camera are rendered first.

case increasingID

Particles with lower IDs are rendered first

case unsorted

Particles are not sorted; they may be rendered in any order.

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

