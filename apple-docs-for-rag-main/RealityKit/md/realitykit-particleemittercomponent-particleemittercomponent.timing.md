

- RealityKit
- ParticleEmitterComponent
-  ParticleEmitterComponent.Timing 

Enumeration

# ParticleEmitterComponent.Timing

Options for specifying the duration of the particle effects, used by the timing property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum Timing
```

## Topics

### Structures

struct VariableDuration

Duration along with an optional variation used to define an amount of time.

### Operators

static func == (ParticleEmitterComponent.Timing, ParticleEmitterComponent.Timing) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case once(warmUp: TimeInterval?, emit: ParticleEmitterComponent.Timing.VariableDuration)

Emits for the given `emit` duration and then stops, `warmUp` determines how long the simulation should appear to have run before first appearing.

case repeating(warmUp: TimeInterval?, emit: ParticleEmitterComponent.Timing.VariableDuration, idle: ParticleEmitterComponent.Timing.VariableDuration?)

Emits for the given `emit` duration, and waits `idle` seconds before looping, `warmUp` determines how long the simulation should appear to have run before first appearing.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable

