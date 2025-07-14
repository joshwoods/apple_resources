

- RealityKit
-  ForceEffectParameters 

Structure

# ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ForceEffectParameters
```

## Topics

### Instance Properties

let angularVelocities: UnsafeForceEffectBuffer&lt;SIMD3&lt;Float>>?

The angular velocities of all rigid bodies under the influence of the effect, or nil if angular velocity information was not requested.

let distances: UnsafeForceEffectBuffer&lt;Float>?

The distance from the effect to each rigid body’s center of mass, or nil if distance information was not requested.

let elapsedTime: TimeInterval

The amount of time that has elapsed since the force effect was started.

let entity: Entity

The entity containing the force effect.

let fixedDeltaTime: TimeInterval

The fixed delta time between simulation steps.

let inertiaTensors: UnsafeForceEffectBuffer&lt;simd_float3x3>?

The inertia tensor based on the current rigid body’s orientation, or nil if inertia tensor information was not requested.

let masses: UnsafeForceEffectBuffer&lt;Float>?

The mass of each rigid body, or nil if mass information was not requested or force mode does not require it.

let orientations: UnsafeForceEffectBuffer&lt;simd_quatf>?

The orientations of all rigid bodies under the influence of the effect, or nil if rotational information was not requested.

let physicsBodyCount: Int

The number of physics bodies to be updated.

let positions: UnsafeForceEffectBuffer&lt;SIMD3&lt;Float>>?

The positions of all rigid bodies under the influence of the effect, or nil if positional information was not requested.

let velocities: UnsafeForceEffectBuffer&lt;SIMD3&lt;Float>>?

The velocities of all rigid bodies under the influence of the effect, or nil if velocity information was not requested.

### Instance Methods

func setForce(SIMD3&lt;Float>, index: Int)

Sets the force for each rigid body.

func setTorque(SIMD3&lt;Float>, index: Int)

Sets the torque for each rigid body.

## See Also

### Custom forces

protocol ForceEffectProtocol

A protocol that defines a custom force effect.

enum ForceMode

The options that control how physics system applies the forces.

protocol ForceEffectBase

The base protocol for the wrapping force effect structure containing common parameters for all force-effects.

