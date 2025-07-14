

- RealityKit
-  PhysicsJointsComponent 

Structure

# PhysicsJointsComponent

A component that stores physics joints which RealityKit simulates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PhysicsJointsComponent
```

## Overview

Add this component to an entity, or any child of an entity, that has a PhysicsSimulationComponent. All joints in the `PhysicsJointsComponent` need to reference entities under the same PhysicsSimulationComponent tree.

Add a joint to the correct `PhysicsJointsComponent` instance by calling its `PhysicsJoint/addToSimulation()-886c4` method.

## Topics

### Operators

static func == (PhysicsJointsComponent, PhysicsJointsComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

Creates a new physics joints component.

### Instance Properties

var joints: PhysicsJoints

The set of joints the physics joints component stores.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Pin and joint components

Simulating physics joints in your RealityKit app

Create realistic, connected motion using physics joints.

struct GeometricPin

A structure that identifies a local transform relative to an entity or entity’s animating skeletal joint.

struct GeometricPinsComponent

A component that stores a sequence of geometric pins.

protocol PhysicsJoint

A type that describes physics joints.

struct EntityGeometricPins

A structure that wraps all geometric pins an entity owns.

