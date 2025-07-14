

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.ParticleEmitter
-  ParticleEmitterComponent.ParticleEmitter.ParticleColor 

Enumeration

# ParticleEmitterComponent.ParticleEmitter.ParticleColor

Options for specifying the behavior of the color of the particles.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum ParticleColor
```

## Topics

### Operators

static func == (ParticleEmitterComponent.ParticleEmitter.ParticleColor, ParticleEmitterComponent.ParticleEmitter.ParticleColor) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case constant(ParticleEmitterComponent.ParticleEmitter.ParticleColor.ColorValue)

The particle will remain the given color throughout its lifetime.

case evolving(start: ParticleEmitterComponent.ParticleEmitter.ParticleColor.ColorValue, end: ParticleEmitterComponent.ParticleEmitter.ParticleColor.ColorValue)

The particle’s color will start at the `start` color and transition over its lifetime to the `end` color.

### Enumerations

enum ColorValue

Options for specifying whether the particle color is a single color, or if the particle should take a random color in the given range.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

