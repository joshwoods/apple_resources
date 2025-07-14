

- SceneKit
-  SCNPhysicsBehavior 

Class

# SCNPhysicsBehavior

The abstract superclass for joints, vehicle simulations, and other high-level behaviors that incorporate multiple physics bodies.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsBehavior
```

## Overview

An SCNPhysicsBehavior object defines a high-level behavior for one or more physics bodies, modifying the results of the physics simulation. Behaviors include joints that connect multiple bodies so they move together and vehicle definitions that cause a body to roll like a car. You never use this class directly; instead, you instantiate one of the subclasses that defines the kind of behavior you want to add to your physics world. describes the kinds of behaviors you can create in SceneKit.

| Class Name | Description |
|----|----|
| SCNPhysicsHingeJoint | Connects two bodies and allows them to pivot around each other on a single axis. |
| SCNPhysicsBallSocketJoint | Connects two bodies and allows them to pivot around each other in any direction. |
| SCNPhysicsSliderJoint | Connects two bodies and allows them to slide or rotate relative to one another. Slider joints can also work as motors, applying a force or torque between the two bodies. |
| SCNPhysicsVehicle | Simulates a physics body as the chassis of a car or other wheeled vehicle. You control a vehicle in terms of steering, braking, and acceleration, and use SCNPhysicsVehicleWheel objects to define the appearance and physical properties of each of its wheels. |

To use a physics behavior, you follow these steps:

1.  Create SCNPhysicsBody objects and attach them to each node that participates in the behavior.

2.  Create and configure a behavior object using one of the subclasses listed in Table 1.

3.  Add the behavior to the physics simulation by calling the addBehavior(_:) method on your scene’s SCNPhysicsWorld object.

## Relationships

### Inherits From

- NSObject

### Inherited By

- SCNPhysicsBallSocketJoint
- SCNPhysicsConeTwistJoint
- SCNPhysicsHingeJoint
- SCNPhysicsSliderJoint
- SCNPhysicsVehicle

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Physics in a Scene

class SCNPhysicsWorld

The global simulation of collisions, gravity, joints, and other physics effects in a scene.

class SCNPhysicsField

An object that applies forces, such as gravitation, electromagnetism, and turbulence, to physics bodies within a certain area of effect.

