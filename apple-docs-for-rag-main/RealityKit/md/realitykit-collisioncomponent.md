

- RealityKit
-  CollisionComponent 

Structure

# CollisionComponent

A component that gives an entity the ability to collide with other entities that also have collision components.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct CollisionComponent
```

## Overview

This component holds the entity’s data related to participating in the scene’s physics simulation. It is also used to calculate collision queries, raycasts, and convex shape casts. Entities can participate in the scene simulation in two different modes: as a *rigid body* or as a *trigger*. A rigid body fully participates in the collision simulation. It affects the velocity and direction of entities it collides. If configured with a rigid body mode of PhysicsBodyMode.dynamic, it’s own velocity and direction can be affected by other rigid body entities. A trigger entity doesn’t have any impact on the rigid bodies in the scene, but can trigger code or Reality Composer behaviors when a rigid body entity overlaps it.

Note the following when considering applying a non-uniform scale to an entity:

- Non-uniform scaling is applicable only to box, convex mesh and triangle mesh collision shapes.

- Non-uniform scaling is not supported for all other types of collision shapes. In this case the scale.x value is duplicated to the scale’s y and z components as well to force scale uniformity based on the x component.

- If the entity has a non-uniform scale assigned to its transform then that entity should not have any descendants assigned that contain rotations in their transforms. A good rule of thumb is to assign the non-uniform scale to the entity that has the collision shape, and avoid adding children below that entity.

Turn an entity into a trigger by adding a CollisionComponent to it and setting its mode to CollisionComponent.Mode.trigger.

Turn an entity into a *rigid body* by adding a PhysicsBodyComponent to the entity in addition to a CollisionComponent. The PhysicsBodyComponent defines the physical properties of the entity, such as its mass and collision shape.

The `filter` property defines the entity’s collision filter, which determines which other objects the entity collides with. For more information, see Controlling Entity Collisions in RealityKit.

Note

If an entity has a PhysicsBodyComponent, the collision component’s mode is ignored. An entity can be a rigid body, or a trigger, but not both at the same time.

## Topics

### Creating the collision component

init(shapes: [ShapeResource], mode: CollisionComponent.Mode, filter: CollisionFilter)

Creates a collision component with the given collision shape, mode, and filter parameters.

### Setting the collision mode

var mode: CollisionComponent.Mode

The collision mode.

### Filtering collisions

var filter: CollisionFilter

The collision filter used to segregate entities into different collision groups.

### Setting collision shapes

var shapes: [ShapeResource]

A collection of shape resources that collectively represent the outer dimensions of an entity for the purposes of collision detection.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Comparing collision components

static func == (CollisionComponent, CollisionComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Structures

struct CollisionOptions

The options set that defines how a collision object reports collisions.

### Initializers

init(shapes: [ShapeResource], isStatic: Bool, filter: CollisionFilter)

Creates a collision component.

init(shapes: [ShapeResource], mode: CollisionComponent.Mode, collisionOptions: CollisionComponent.CollisionOptions, filter: CollisionFilter)

### Instance Properties

var collisionOptions: CollisionComponent.CollisionOptions

var isStatic: Bool

A Boolean value that indicates whether the collider is static.

### Enumerations

enum Mode

A mode that dictates how much collision data is collected for a given entity.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Collision shapes and groups

Simulating physics with collisions in your visionOS app

Create entities that behave and react like physical objects in a RealityKit view.

Configuring Collision in RealityKit

Use collision groups and collision filters to control which objects collide.

enum Mode

A mode that dictates how much collision data is collected for a given entity.

class ShapeResource

A representation of a shape.

enum ShapeResourceError

struct CollisionGroup

A bitmask used to define the collision group to which an entity belongs.

struct CollisionFilter

A set of masks that determine whether entities can collide during simulations.

class TriggerVolume

An invisible 3D shape that detects when objects enter or exit a given region of space.

