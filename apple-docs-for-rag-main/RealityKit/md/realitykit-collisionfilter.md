

- RealityKit
-  CollisionFilter 

Structure

# CollisionFilter

A set of masks that determine whether entities can collide during simulations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct CollisionFilter
```

## Overview

Use Collision filters in combination with collision groups to define which entities collide with which other entities in a scene. For more information on using collision filters, see CollisionGroup

## Topics

### Creating a collision filter

init(group: CollisionGroup, mask: CollisionGroup)

Creates a collision filter.

static let `default`: CollisionFilter

The default collision filter.

static let sensor: CollisionFilter

A collision filter for an entity that collides with everything.

### Customizing groups

var group: CollisionGroup

The collision group or groups, stored as a bit mask, to which the entity belongs.

var mask: CollisionGroup

The collision group or groups, stored as a bitmask, with which the entity can collide.

### Comparing collision filters

static func == (CollisionFilter, CollisionFilter) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

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

class TriggerVolume

An invisible 3D shape that detects when objects enter or exit a given region of space.

