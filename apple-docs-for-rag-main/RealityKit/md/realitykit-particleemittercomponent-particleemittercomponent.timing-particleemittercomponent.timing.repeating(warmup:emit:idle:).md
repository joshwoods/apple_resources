

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.Timing
-  ParticleEmitterComponent.Timing.repeating(warmUp:emit:idle:) 

Case

# ParticleEmitterComponent.Timing.repeating(warmUp:emit:idle:)

Emits for the given `emit` duration, and waits `idle` seconds before looping, `warmUp` determines how long the simulation should appear to have run before first appearing.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
case repeating(
    warmUp: TimeInterval? = nil,
    emit: ParticleEmitterComponent.Timing.VariableDuration,
    idle: ParticleEmitterComponent.Timing.VariableDuration? = nil
)
```

