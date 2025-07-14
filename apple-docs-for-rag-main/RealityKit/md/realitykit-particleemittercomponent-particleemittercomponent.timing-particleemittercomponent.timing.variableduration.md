

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.Timing
-  ParticleEmitterComponent.Timing.VariableDuration 

Structure

# ParticleEmitterComponent.Timing.VariableDuration

Duration along with an optional variation used to define an amount of time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct VariableDuration
```

## Topics

### Operators

static func == (ParticleEmitterComponent.Timing.VariableDuration, ParticleEmitterComponent.Timing.VariableDuration) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(duration: TimeInterval, variation: TimeInterval?)

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

let duration: TimeInterval

Base duration of time.

let variation: TimeInterval?

Defines a plus/minus range from which a value is randomly selected and used to offset duration.

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

