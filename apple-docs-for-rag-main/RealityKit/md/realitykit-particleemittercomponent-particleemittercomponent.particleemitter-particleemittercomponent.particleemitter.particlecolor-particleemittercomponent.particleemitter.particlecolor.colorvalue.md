

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.ParticleEmitter
- ParticleEmitterComponent.ParticleEmitter.ParticleColor
-  ParticleEmitterComponent.ParticleEmitter.ParticleColor.ColorValue 

Enumeration

# ParticleEmitterComponent.ParticleEmitter.ParticleColor.ColorValue

Options for specifying whether the particle color is a single color, or if the particle should take a random color in the given range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum ColorValue
```

## Topics

### Operators

static func == (ParticleEmitterComponent.ParticleEmitter.ParticleColor.ColorValue, ParticleEmitterComponent.ParticleEmitter.ParticleColor.ColorValue) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case random(a: ParticleEmitterComponent.ParticleEmitter.Color, b: ParticleEmitterComponent.ParticleEmitter.Color)

The system will choose a random color for each particle between the given two Colors.

case random(a: ParticleEmitterComponent.ParticleEmitter.Color, b: ParticleEmitterComponent.ParticleEmitter.Color)

The system will choose a random color for each particle between the given two Colors.

case single(ParticleEmitterComponent.ParticleEmitter.Color)

The particle will be the given Color.

case single(ParticleEmitterComponent.ParticleEmitter.Color)

The particle will be the given Color.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

