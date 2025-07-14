

- RealityKit
-  PhysicsMotionComponent 

Structure

# PhysicsMotionComponent

A component that controls the motion of the body in physics simulations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct PhysicsMotionComponent
```

## Mentioned in 

Designing scene hierarchies for efficient physics simulation

## Overview

You specify velocities in the coordinate space of the physics simulation defined by nearestSimulationEntity(for:).

The behavior of an entity with a physics motion component depends on the entity’s mode setting:

PhysicsBodyMode.static  
The physics simulation ignores the velocities. The entity doesn’t move.

PhysicsBodyMode.kinematic  
The physics simulation moves the body according to the values you set for angularVelocity and linearVelocity.

PhysicsBodyMode.dynamic  
The physics simulation overwrites the velocity values based on simulation, and ignores any values that you write.

## Topics

### Creating the motion component

init()

Creates a physics motion component at rest.

init(linearVelocity: SIMD3&lt;Float>, angularVelocity: SIMD3&lt;Float>)

Creates a physics motion component with the given velocities.

### Setting velocity

var angularVelocity: SIMD3&lt;Float>

The angular velocity of the body around the center of mass.

var linearVelocity: SIMD3&lt;Float>

The linear velocity of the body in the physics simulation.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Comparing physics motion components

static func == (PhysicsMotionComponent, PhysicsMotionComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Physics motion

struct ImpulseAction

An action that applies an impulse to the physics body at its center of mass when played as an animation.

