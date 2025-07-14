

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.Timing
-  ParticleEmitterComponent.Timing.once(warmUp:emit:) 

Case

# ParticleEmitterComponent.Timing.once(warmUp:emit:)

Emits for the given `emit` duration and then stops, `warmUp` determines how long the simulation should appear to have run before first appearing.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
case once(
    warmUp: TimeInterval? = nil,
    emit: ParticleEmitterComponent.Timing.VariableDuration
)
```

