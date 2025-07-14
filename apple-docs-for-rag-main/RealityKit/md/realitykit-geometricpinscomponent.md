

- RealityKit
-  GeometricPinsComponent 

Structure

# GeometricPinsComponent

A component that stores a sequence of geometric pins.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct GeometricPinsComponent
```

## Overview

Add, inspect, and remove geometric pins that belong to the entity that owns an instance of `GeometricPinsComponent` by accessing its pins property.

## Topics

### Initializers

init()

Creates a geometric pins component with an empty sequence of pins.

### Instance Properties

var pins: Set&lt;GeometricPin>

The sequence of geometric pins the component owns.

### Instance Methods

func removePin(named: String) -> GeometricPin?

Removes the pin associated with the name.

func set(pin: GeometricPin)

Adds a pin to the collection.

### Subscripts

subscript(String) -> GeometricPin?

Retrieves the pin by its name.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Pin and joint components

Simulating physics joints in your RealityKit app

Create realistic, connected motion using physics joints.

struct GeometricPin

A structure that identifies a local transform relative to an entity or entity’s animating skeletal joint.

protocol PhysicsJoint

A type that describes physics joints.

struct PhysicsJointsComponent

A component that stores physics joints which RealityKit simulates.

struct EntityGeometricPins

A structure that wraps all geometric pins an entity owns.

