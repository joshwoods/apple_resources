

- RealityKit
- CollisionComponent
-  CollisionComponent.Mode 

Enumeration

# CollisionComponent.Mode

A mode that dictates how much collision data is collected for a given entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
enum Mode
```

## Topics

### Collision modes

case `default`

A default collision object.

case trigger

A trigger collision object.

### Comparing collision modes

static func == (CollisionComponent.Mode, CollisionComponent.Mode) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Enumeration Cases

case colliding

An environmental collision object.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Collision shapes and groups

Simulating physics with collisions in your visionOS app

Create entities that behave and react like physical objects in a RealityKit view.

Configuring Collision in RealityKit

Use collision groups and collision filters to control which objects collide.

struct CollisionComponent

A component that gives an entity the ability to collide with other entities that also have collision components.

class ShapeResource

A representation of a shape.

enum ShapeResourceError

struct CollisionGroup

A bitmask used to define the collision group to which an entity belongs.

struct CollisionFilter

A set of masks that determine whether entities can collide during simulations.

class TriggerVolume

An invisible 3D shape that detects when objects enter or exit a given region of space.

