

- RealityKit
-  CollisionGroup 

Structure

# CollisionGroup

A bitmask used to define the collision group to which an entity belongs.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct CollisionGroup
```

## Overview

Use collision groups along with CollisionFilter to define custom collision properties for entities in your scene and to control which entities collide with which others. By default, all entities that participate in the physics simulation collide with all other participating entities. There are times, however, when you need certain entities to not collide with certain other entities, and that’s where collision groups and filters come into play.

Create individual collision groups using raw bit flag values, like this:

```
let redGroup = CollisionGroup(rawValue: 1 

Because CollisionGroup conforms to OptionSet, this allows you to create aggregate groups that encompass multiple individual collision groups, like so:

```
let blueAndRedGroup = redGroup.union(blueGroup)
let greenAndYellowGroup = greenGroup.union(yellowGroup)
```

You can also define groups that have all entities except those in specific groups. In a game, for example, you might want to turn off collisions between members of the same team or between pieces owned by the same player. This is what creating that kind of filter would look like:

```
let allButRedGroup = CollisionGroup.all.subtracting(redGroup)
```

Collision groups aren’t assigned directly to entities. Instead, you create a CollisionFilter for the group, and then assign that filter to all the entities you wish to include in its group. The collision filter’s mask defines which objects the entities in this group collide with, and all entities that share the same filter are part of the same collision group.

```
let allButRedFilter = CollisionFilter(group: redGroup, mask: allButRedGroup)
redTeamPlayer1.collision?.filter = allButRedFilter
```

## Topics

### Standard collision groups

static let `default`: CollisionGroup

The default collision group for objects.

static let all: CollisionGroup

The collision group that represents all groups.

static let sceneUnderstanding: CollisionGroup

The default collision group for scene-understanding meshes.

### Creating a collision group

init()

Creates an empty option set.

init(rawValue: UInt32)

Creates a collision group from a raw value.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

### Option set

let rawValue: UInt32

The corresponding value of the raw type.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

typealias Element

The element type of the option set.

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

let rawValue: UInt32

The corresponding value of the raw type.

func contains(Self) -> Bool

Returns a Boolean value that indicates whether a given element is a member of the option set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func formSymmetricDifference(Self)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

func formUnion(Self)

Inserts the elements of another set into this option set.

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

func intersection(Self) -> Self

Returns a new option set with only the elements contained in both this set and the given set.

func isDisjoint(with: Self) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given set.

func isStrictSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

func isStrictSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict superset of the given set.

func isSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a subset of another set.

func isSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given set.

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

func subtract(Self)

Removes the elements of the given set from this set.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

func symmetricDifference(Self) -> Self

Returns a new option set with the elements contained in this set or in the given set, but not in both.

func union(Self) -> Self

Returns a new option set of the elements contained in this set, in the given set, or in both.

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

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

struct CollisionFilter

A set of masks that determine whether entities can collide during simulations.

class TriggerVolume

An invisible 3D shape that detects when objects enter or exit a given region of space.

