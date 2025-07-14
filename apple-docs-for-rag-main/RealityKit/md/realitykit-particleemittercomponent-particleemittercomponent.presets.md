

- RealityKit
- ParticleEmitterComponent
-  ParticleEmitterComponent.Presets 

Structure

# ParticleEmitterComponent.Presets

Initial configurations that can be set when starting a new simulation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Presets
```

## Topics

### Type Properties

static var fireworks: ParticleEmitterComponent

Particles that emit in regular bursts and spawn secondary particles

static var impact: ParticleEmitterComponent

Particles that emit in a radial pattern and simulate dust from an object hitting the ground

static var magic: ParticleEmitterComponent

Particles that twinkle and emit spawn particles

static var rain: ParticleEmitterComponent

Fast, semi-opaque particles rendered as streaks

static var snow: ParticleEmitterComponent

Softly falling particles that incorporate motion from a noise pattern

static var sparks: ParticleEmitterComponent

Quick and short lived particles that accumulate color to simulate welding sparks

## See Also

### Particle simulation

Simulating particles in your visionOS app

Add a range of visual effects to a RealityKit view by attaching a particle emitter component to an entity.

struct ParticleEmitterComponent

A component that emits particles.

struct ParticleEmitter

