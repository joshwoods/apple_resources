

- RealityKit
-  TriggerVolume 

Class

# TriggerVolume

An invisible 3D shape that detects when objects enter or exit a given region of space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class TriggerVolume
```

## Overview

A trigger volume is an entity that can participate in collisions because it has a CollisionComponent. You use a trigger volume as a sensor that indicates when another collision-capable entity, like a ModelEntity, enters the region of space occupied by the trigger volume. You can use the generated CollisionEvents between the trigger volume and the other entity to trigger an action, like indicating to the user that a projectile hit its target.

The trigger volume itself is very simple. It lacks any physical appearance, and doesn’t participate in physics simulations. This makes it very efficient for tasks that require only collision detection.

## Topics

### Creating a trigger volume

init()

Creates a trigger volume.

convenience init(shape: ShapeResource, filter: CollisionFilter)

Creates a trigger volume with the given shape and collision filter.

init(shapes: [ShapeResource], filter: CollisionFilter)

Creates a trigger volume with the given composite shape and collision filter.

### Detecting collisions

var collision: CollisionComponent?

The collision component that gives the entity the ability to participate in collision simulations.

### Default Implementations

HasCollision Implementations

## Relationships

### Inherits From

- Entity

### Conforms To

- CustomDebugStringConvertible
- Equatable
- EventSource
- HasCollision
- HasHierarchy
- HasSynchronization
- HasTransform
- Hashable
- Identifiable
- RealityCoordinateSpace
- Sendable

## See Also

### Collision shapes and groups

Simulating physics with collisions in your visionOS app

Create entities that behave and react like physical objects in a RealityKit view.

Configuring Collision in RealityKit

Use collision groups and collision filters to control which objects collide.

struct CollisionComponent

A component that gives an entity the ability to collide with other entities that also have collision components.

enum Mode

A mode that dictates how much collision data is collected for a given entity.

class ShapeResource

A representation of a shape.

enum ShapeResourceError

struct CollisionGroup

A bitmask used to define the collision group to which an entity belongs.

struct CollisionFilter

A set of masks that determine whether entities can collide during simulations.

