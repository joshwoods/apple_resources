

- RealityKit
-  PhysicsSimulationComponent 

Structure

# PhysicsSimulationComponent

A component that controls localized physics simulations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct PhysicsSimulationComponent
```

## Overview

Simulate local physics by adding a PhysicsSimulationComponent to an entity. The component gives your app the ability to customize the physics simulation by configuring its properties, such as gravity and collisionOptions.

Important

Each physics simulation component uses meters as its unit of distance, which can be important to other types in the physics simulation, such as ShapeResource instances.

## Topics

### Structures

struct CollisionOptions

The options set that defines how a physics simulation reports collisions.

struct SolverIterations

The parameters that control the accuracy of solving physics simulations.

### Operators

static func == (PhysicsSimulationComponent, PhysicsSimulationComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

### Instance Properties

var clock: CMClockOrTimebase

A custom clock which drives the physics simulation, defaults to the engine clock.

var collisionOptions: PhysicsSimulationComponent.CollisionOptions

Options for kinematic collision reporting.

var gravity: SIMD3&lt;Float>

The gravity for the simulation relative to the simulation entity.

var solverIterations: PhysicsSimulationComponent.SolverIterations

The parameters that control the accuracy of solving physics simulations.

### Type Methods

static func nearestSimulationEntity(for: Entity) -> Entity?

Obtains the entity containing the physics simulation origin.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Simulation setup

Designing scene hierarchies for efficient physics simulation

Configure your RealityKit scenes to avoid performance bottlenecks.

Handling different-sized objects in physics simulations

Set up a scene hierarchy for accurate physics simulations.

