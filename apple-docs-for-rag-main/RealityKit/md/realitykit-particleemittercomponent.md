

- RealityKit
-  ParticleEmitterComponent 

Structure

# ParticleEmitterComponent

A component that emits particles.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct ParticleEmitterComponent
```

## Overview

To learn how to use `ParticleEmitterComponent` in your app, see Simulating particles in your visionOS app.

## Topics

### Structures

struct ParticleEmitter

struct Presets

Initial configurations that can be set when starting a new simulation.

### Initializers

init()

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var birthDirection: ParticleEmitterComponent.BirthDirection

The possible initial directions for newly spawned particles, relative to the emitter shape.Defaults to normal.

var birthLocation: ParticleEmitterComponent.BirthLocation

The possible locations for newly spawned particles, relative to the emitter shape. Defaults to surface.

var burstCount: Int

Number of particles to emit in a single burst. Defaults to 100.

var burstCountVariation: Int

Defines a plus/minus range from which a value is randomly selected to offset `burstCount`.

var emissionDirection: SIMD3&lt;Float>

The direction particles are emitted when birthDirection is set to World or Local. Defaults to (0.0, 1.0, 0.0).

var emitterShape: ParticleEmitterComponent.EmitterShape

The shape of the region of space where the system spawns new particles. Defaults to plane.

var emitterShapeSize: SIMD3&lt;Float>

The emitter shape size in meters.

var fieldSimulationSpace: ParticleEmitterComponent.SimulationSpace

Field Simulation Space, either local or global

var isEmitting: Bool

Disables/enables particle emission, independent of `simulationState`. Existing particles will not be affected.

var mainEmitter: ParticleEmitterComponent.ParticleEmitter

Particle attributes affecting the main particles of the base simulation.

var particlesInheritTransform: Bool

Determines if the entity’s transformation also affects the particles.

var radialAmount: Float

Radial sweep angle for sphere, cylinder, cone, and torus emitter shapes. Defaults to 2 \* pi.

var simulationState: ParticleEmitterComponent.SimulationState

Controls particle simulation state: playing, paused or stopped. Defaults to `play`.

var spawnInheritsParentColor: Bool

Whether or not the spawnedEmitter’s color should be overriden by the mainEmitter’s color at the time of the spawning.

var spawnOccasion: ParticleEmitterComponent.SpawnOccasion

Determines when main particles emit spawn particles. Defaults to `onDeath`.

var spawnSpreadFactor: Float

Amount a spawned particle spreads away from its parent particle, works in conjunction with the spawn particle’s `spreadingAngle`. Defaults to 0.

var spawnSpreadFactorVariation: Float

Defines a plus/minus range from which a value is randomly selected to offset Spawn Spread Factor.

var spawnVelocityFactor: Float

How much of the parent particle’s velocity to inherit. Defaults to 1.

var spawnedEmitter: ParticleEmitterComponent.ParticleEmitter?

Attributes affecting secondary particles spawned from the main simulation.

var speed: Float

The initial speed, in meters per second, for newly spawned particles. Defaults to 0.5.

var speedVariation: Float

Defines a plus/minus range (in meters per second) from which a value is randomly selected to offset particle speed.

var timing: ParticleEmitterComponent.Timing

Defines the Emitter timing method.

var torusInnerRadius: Float

Radius of the torus’ emitter shape tube. Defaults to 0.25.

### Instance Methods

func burst()

Emits burstCount particles on the next update call.

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func restart()

Restarts the emission of particles. Requires the component to be re-assigned to the entity to take effect.

### Enumerations

enum BirthDirection

Options for the initial direction of each emitted particle, used by the birthDirection property.

enum BirthLocation

Options for the location on the shape of where particles are born, used by the birthLocation property.

enum EmitterShape

Options for the shape of an emitter, used by the emitterShape property.

enum SimulationSpace

Options for particle simulation space

enum SimulationState

Options for the particle simulation state, used by the `simulationState` property.

enum SpawnOccasion

Options for when the spawned effect starts, used by the spawnOccasion property.

enum Timing

Options for specifying the duration of the particle effects, used by the timing property.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component
- Decodable
- Encodable

## See Also

### Particle simulation

Simulating particles in your visionOS app

Add a range of visual effects to a RealityKit view by attaching a particle emitter component to an entity.

struct ParticleEmitter

struct Presets

Initial configurations that can be set when starting a new simulation.

