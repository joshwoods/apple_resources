

- RealityKit
- ParticleEmitterComponent
-  ParticleEmitterComponent.SimulationState 

Enumeration

# ParticleEmitterComponent.SimulationState

Options for the particle simulation state, used by the `simulationState` property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum SimulationState
```

## Topics

### Operators

static func == (ParticleEmitterComponent.SimulationState, ParticleEmitterComponent.SimulationState) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case pause

Simulation will pause.

case play

Simulation will play.

case stop

Simulation will stop and clear existing particles.

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

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable

