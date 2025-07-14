

- RealityKit
-  GeometricPin 

Structure

# GeometricPin

A structure that identifies a local transform relative to an entity or entity’s animating skeletal joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct GeometricPin
```

## Overview

A geometric pin has a base transform and allows an optional offset relative to the base transform. The base transform is only available when the pin attaches to an entity. When a geometric pin does not attach to any entity (i.e. `GeometricPin/entity` is `nil`), the pin is just a floating local transform relative to some space to be defined. The pin’s query function such as `GeometricPin/position` or `GeometricPin/orientation` returns the local offset in this case.

After a geometric pin has attached to an entity, or `GeometricPin/entity` is not `nil`, the base transform may be available. If you construct a geometric pin with a generic name, the base transform resolves to the transform of the pin’s owning entity. If you construct a geometric pin with a skeletal joint name, the base transform resolves to the current transform of the skeletal joint with the matching joint name. When the base transform is available, the pin’s query function such as `GeometricPin/position` or `GeometricPin/orientation` returns the base transform with the offset applied.

You can attach a pin to an entity by creating a `GeometricPin`, adding it to a GeometricPinsComponent, and finally setting the GeometricPinsComponent to an `Entity`.

```
let pin = GeometricPin(named: "genericPin")
let skeletalJointPin = GeometricPin(named: "animatingPin", skeletalJointName: "hand")
var pinsComponent = GeometricPinsComponent()
pinsComponent.set(pin)
pinsComponent.set(skeletalJointPin)
let entity = Entity()
entity.components.set(pinsComponent)
```

Another way to attach a pin is to add the `GeometricPin` to the pins collection directly.

```
let entity = Entity()
let pin = entity.pins.set(named: "genericPin")
let skeletalJointPin = entity.pins.set(named: "animatingPin", skeletalJointName: "hand")
```

Note that when adding a geometric pin the API does not validate the skeletal joint name. The validation only happens when the base transform is evaluating, for example during the call to `GeometricPin/position` or `GeometricPin/orientation`. If the skeletal joint name does not match any valid skeletal joint, those query functions return `nil`.

Each geometric pin has a unique name to identify itself from other pins on an entity. You can use the subscript operator to retrieve a pin.

```
// To retrieve the skeletal joint pin in the previous snippet:
let retrievedPin = pinsComponent["animatingPin"]
```

## Topics

### Operators

static func == (GeometricPin, GeometricPin) -> Bool

Returns a Boolean that indicates whether the pins are equal.

### Initializers

init(named: String, offsetPosition: SIMD3&lt;Float>, offsetOrientation: simd_quatf)

Creates a geometric pin that identifies a local position and orientation.

init(named: String, skeletalJointName: String, offsetPosition: SIMD3&lt;Float>, offsetOrientation: simd_quatf)

Creates a geometric pin that attaches to a skeletal joint.

### Instance Properties

var entity: Entity?

The entity where the local frame lives.

var hashValue: Int

The hash value.

var name: String

The name of the pin.

var offsetOrientation: simd_quatf

Offset from the pin’s base orientation.

var offsetPosition: SIMD3&lt;Float>

Offset from the pin’s base position.

var orientation: simd_quatf?

Calculates and returns the current orientation of the pin relative to the pin’s owning entity, adjusted by the optional offset orientation.

var position: SIMD3&lt;Float>?

Calculates and returns the current position of the pin relative to the pin’s owning entity, adjusted by the optional offset position.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of the pin by feeding them into the hash function.

func orientation(relativeTo: Entity?) -> simd_quatf?

Calculates and returns the current orientation of the pin relative to a reference entity, adjusted by the optional offset position.

func position(relativeTo: Entity?) -> SIMD3&lt;Float>?

Calculates and returns the current position of the pin relative to a reference entity, adjusted by the optional offset position.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Pin and joint components

Simulating physics joints in your RealityKit app

Create realistic, connected motion using physics joints.

struct GeometricPinsComponent

A component that stores a sequence of geometric pins.

protocol PhysicsJoint

A type that describes physics joints.

struct PhysicsJointsComponent

A component that stores physics joints which RealityKit simulates.

struct EntityGeometricPins

A structure that wraps all geometric pins an entity owns.

