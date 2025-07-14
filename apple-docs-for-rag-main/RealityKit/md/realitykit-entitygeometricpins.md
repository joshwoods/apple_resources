

- RealityKit
-  EntityGeometricPins 

Structure

# EntityGeometricPins

A structure that wraps all geometric pins an entity owns.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
struct EntityGeometricPins
```

## Overview

Access an instance of this structure through the entity property pins.

## Topics

### Structures

struct Iterator

An object to iterate over all geometric pins in the collection.

### Instance Properties

var count: Int

The total number of pins.

let entity: Entity

The entity where the local frame lives.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

### Instance Methods

func makeIterator() -> EntityGeometricPins.Iterator

Returns an iterator for the sequence.

func remove(named: String)

Removes a geometric pin with the given name from this entity.

func set(named: String, position: SIMD3&lt;Float>, orientation: simd_quatf) -> GeometricPin

Creates and adds a geometric pin to the entity, and returns the entity geometric pin.

func set(named: String, position: SIMD3&lt;Float>, orientation: simd_quatf, relativeTo: Entity?) -> GeometricPin

Creates and adds a geometric pin to the entity, and returns the entity geometric pin.

func set(named: String, skeletalJointName: String, position: SIMD3&lt;Float>, orientation: simd_quatf) -> GeometricPin

Creates and adds a geometric pin to the entity’s skeletal joint, and returns the geometric pin.

### Subscripts

subscript(String) -> GeometricPin?

Obtains a geometric pin the entity owns by name.

### Type Aliases

typealias Element

An individual pin in the collection.

### Default Implementations

Sequence Implementations

## Relationships

### Conforms To

- Sendable
- Sequence

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

struct PhysicsJointsComponent

A component that stores physics joints which RealityKit simulates.

