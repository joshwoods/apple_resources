

- RealityKit
- ParticleEmitterComponent
-  ParticleEmitterComponent.ParticleEmitter 

Structure

# ParticleEmitterComponent.ParticleEmitter

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct ParticleEmitter
```

## Topics

### Structures

struct ImageSequence

Structure used to define properties of the sprite sheet, used by imageSequence.

### Initializers

init()

### Instance Properties

var acceleration: SIMD3&lt;Float>

The constant acceleration vector, in meters per second squared, applied to all particles in the system.

var angle: Float

The rotation angle, in radians, of newly spawned particles. Defaults to 0.

var angleVariation: Float

Defines a plus/minus range (in radians) from which a value is randomly selected to offset `angle`.

var angularSpeed: Float

The initial spin rate, in radians per second, of newly spawned particles. Defaults to 0.

var angularSpeedVariation: Float

Defines a plus/minus range (in radians per second) from which a value is randomly selected to offset `angularSpeed`.

var attractionCenter: SIMD3&lt;Float>

The spot that the particles are attracted to. In local space. Defaults to (1, 1, 0).

var attractionStrength: Float

The particles are attracted to the `attractionCenter` by this amount. Defaults to 0.

var billboardMode: ParticleEmitterComponent.ParticleEmitter.BillboardMode

The mode defining whether and how particles orient towards the camera. Defaults to `billboardYAligned`.

var birthRate: Float

The number of particles emitted over the emission duration. Defaults to 100.

var birthRateVariation: Float

Defines a plus/minus range from which a value is randomly selected to offset `birthRate`.

var blendMode: ParticleEmitterComponent.ParticleEmitter.BlendMode

How overlapping particles are composited together. Defaults to `alpha`.

var color: ParticleEmitterComponent.ParticleEmitter.ParticleColor

The color of particles.

var colorEvolutionPower: Float

How quickly the color evolves from its start to its end color — a value of 1 is a linear transition, values below 1 transition quicker, values over 1 transition slower.

var dampingFactor: Float

A factor that slows particles relative to their velocity. Defaults to 0.

var image: TextureResource?

The image that each particle will use (requires pre-multiplied RGB values). Defaults to a white circular texture.

var imageSequence: ParticleEmitterComponent.ParticleEmitter.ImageSequence?

Determines if the particle image is a sprite sheet (used for animation).

var isLightingEnabled: Bool

Determines if particles are affected by scene lighting.

var lifeSpan: Double

The duration, in seconds, for which each particle is rendered before being removed from the scene. Defaults to 1.

var lifeSpanVariation: Double

Defines a plus/minus range (in seconds) from which a value is randomly selected to offset `lifeSpan`. Defaults to 0.2.

var mass: Float

The mass, in grams, of each particle in the system. Defaults to 1.

var massVariation: Float

Defines a plus/minus range (in grams) from which a value is randomly selected to offset `mass`.

var noiseAnimationSpeed: Float

Determines how fast the noise field changes over time. Defaults to 0.

var noiseScale: Float

Scale of the noise (turbulence) patterns. Defaults to 1.

var noiseStrength: Float

Strength of the noise (turbulence) fields affecting particle motion. Defaults to 0.

var opacityCurve: ParticleEmitterComponent.ParticleEmitter.OpacityCurve

The curve of opacity change over the lifetime of the particle. Defaults to `quickFadeInOut`.

var size: Float

The rendered size, in units of the scene’s world coordinate space, of the particle image. Value is the half-extent of the particle’s quad. Defaults to 0.02.

var sizeMultiplierAtEndOfLifespan: Float

At the end of the particle lifespan, the particle’s size will be it’s initial size times this multiplier. Defaults to 0.1.

var sizeMultiplierAtEndOfLifespanPower: Float

How quickly or slowly particle size changes over its lifetime — a value of 1 is linear, values below 1 transition quicker, values above 1 transition slower.

var sizeVariation: Float

Defines a plus/minus range from which a value is randomly selected to offset `size`.

var sortOrder: ParticleEmitterComponent.ParticleEmitter.SortOrder

How overlapping particles are sorted before rendering. Defaults to `increasingDepth`.

var spreadingAngle: Float

The range, in radians, of randomized initial particle directions as radians describing the size of the spreading cone. Defaults to 0.

var stretchFactor: Float

How much a particle’s shape is stretched along its velocity direction (Billboard particles only).

var vortexDirection: SIMD3&lt;Float>

Direction vector of the vortex axis. Defaults to (0, 1, 0).

var vortexStrength: Float

Strength of the vortex forces affecting particle motion. Defaults to 0.

### Type Aliases

typealias Color

### Enumerations

enum BillboardMode

Options for specifying the axis about which the particle will be oriented, used by the `billboardMode` property.

enum BlendMode

Options for combining source and destination pixel colors when compositing particles during rendering, used by the blendMode property.

enum OpacityCurve

Options for the curve of opacity change over the lifetime of the particle, used by the opacityOverLife property.

enum ParticleColor

Options for specifying the behavior of the color of the particles.

enum SortOrder

Options for the rendering order of particles, used by the sortingMode property.

### Default Implementations

Decodable Implementations

Encodable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable

## See Also

### Particle simulation

Simulating particles in your visionOS app

Add a range of visual effects to a RealityKit view by attaching a particle emitter component to an entity.

struct ParticleEmitterComponent

A component that emits particles.

struct Presets

Initial configurations that can be set when starting a new simulation.

