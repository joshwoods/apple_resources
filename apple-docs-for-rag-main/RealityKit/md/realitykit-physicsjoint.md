

- RealityKit
-  PhysicsJoint 

Protocol

# PhysicsJoint

A type that describes physics joints.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
protocol PhysicsJoint : Equatable
```

## Overview

`PhysicsJoint` objects are transient and define physics joints properties. PhysicsJointsComponent stores physics joints when added to an entity.

Each `PhysicsJoint` references two entities at local poses (position and orientation) specified on each Entity.

The two pins of a physics joint, pin0 and pin1, each reference poses on the entities that make up each point on a `PhysicsJoint`. Use two unique entities that both have a PhysicsBodyComponent, and belong to the same physics simulation.

Joints specify linear and angular limits of motion, limiting the motion of the second pin (pin1) relative to the first pin (pin0).

To become active, the `PhysicsJoint` needs to be added to a PhysicsJointsComponent This is achieved by either directly on the component, or by calling addToSimulation(). Once you add the joint to the simulation context, you no longer need to reference `PhysicsJoint` directly in your code.

For example, a PhysicsRevoluteJoint that connects a window, `windowEntity`, to a window frame, `frameEntity`:

```
let parentSimulationEntity = Entity()
// Add PhysicsSimulationComponent to parentSimulationEntity...

let frameEntity = Entity()
let windowEntity = Entity()
// Add PhysicsBodyComponents to the entities...

// Create a hinge the references points on the entities.
let windowWidth: Float = 1
let framePin = frameEntity.pins.set(
    named: "FrameHinge",
    // In this example, center of the frame is the center of its bounding box,
    // so the hinge is half its width to the negative x direction.
    position: [-windowWidth / 2, 0, 0],
    // This hinge rotates around the x-axis, but this window needs to
    // rotate around the y-axis.
    // This rotation modifies the pin's positive x-axis to the positive y-axis.
    orientation: simd_quatf(from: [1, 0, 0], to: [0, 1, 0])
)

// Get a previously created GeometricPin from `windowEntity`,
// or a new one create one as above.
let windowPin = GeometricPin(entity: windowEntity, pinName: "WindowHinge")

let windowHingeJoint = PhysicsRevoluteJoint(
    pin0: framePin,
    pin1: windowPin,
    // Allow the hinge to rotate up to 90º.
    angularLimit: 0...Float.pi
)
try windowHingeJoint.addToSimulation()
```

**Best practices:**

- When creating a joint, make sure that the jointed entities are initially positioned so that they satisfy the joint. If not done so, the physics solver may have difficulty bringing the entities together to satisfy the joint.

- When connecting a PhysicsBodyMode.kinematic and a PhysicsBodyMode.dynamic entities by a joint, use pin0 as the pin on the kinematic entity.  
  If both are PhysicsBodyMode.dynamic, set the heavier entity as pin0.

- Aim to make the entities connected by joints similar in mass.

- Add a PhysicsSimulationComponent to a common ancestor when creating `PhysicsJoint` instances, to make it clear which physics simulation is used to solve the joints.

- To improve the the solving of the joints, adjust the value of the solverIterations property.

## Topics

### Instance Properties

var checksForInternalCollisions: Bool

A Boolean that indicates whether the joint checks and reports collisions between the two entity instances.

**Required**

var isActive: Bool

A Boolean that indicates whether the joint is active.

**Required**

var pin0: GeometricPin

The pin that defines a local position and orientation on the first entity.

**Required**

var pin1: GeometricPin

The pin that defines a local position and orientation on the second entity.

**Required**

### Instance Methods

func addToSimulation() throws -> Entity

Adds this joint to the simulation.

## Relationships

### Inherits From

- Equatable

### Conforming Types

- PhysicsCustomJoint
- PhysicsDistanceJoint
- PhysicsFixedJoint
- PhysicsPrismaticJoint
- PhysicsRevoluteJoint
- PhysicsSphericalJoint

## See Also

### Pin and joint components

Simulating physics joints in your RealityKit app

Create realistic, connected motion using physics joints.

struct GeometricPin

A structure that identifies a local transform relative to an entity or entity’s animating skeletal joint.

struct GeometricPinsComponent

A component that stores a sequence of geometric pins.

struct PhysicsJointsComponent

A component that stores physics joints which RealityKit simulates.

struct EntityGeometricPins

A structure that wraps all geometric pins an entity owns.

