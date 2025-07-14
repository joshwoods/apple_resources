

- SceneKit
-  SCNPhysicsVehicleWheel 

Class

# SCNPhysicsVehicleWheel

The appearance and physical characteristics of an individual wheel associated with an physics vehicle behavior.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsVehicleWheel
```

## Overview

To use wheels in a vehicle simulation, include them when creating an SCNPhysicsVehicle object with the init(chassisBody:wheels:) initializer, then add the vehicle object to your scene’s physics world using the physics world’s addBehavior(_:) method.

### Creating a Wheel

You create a wheel with an SCNNode object whose contents provide the wheel’s visual representation—a geometry that rotates when the simulated vehicle rolls along a surface. The node representing a wheel must be a child of the node containing the physics body that serves as the vehicle’s chassis, and each wheel in a vehicle must reference a unique node. Typically, you load a scene file that contains a node hierarchy representing the vehicle and all of its wheels. Next, you designate which nodes serve as the body and wheels.

Because the SCNPhysicsVehicle behavior that a wheel is attached to manages its participation in the physics simulation, you don’t need to attach a physics body to the SCNNode object representing a wheel.

### Changing a Wheel’s Physical Properties

The properties of a wheel define the geometry of its connection to the vehicle and simulate its size, traction, and suspension. You can change these properties after the wheel and the vehicle containing it have been added to the physics world. In this way, you can simulate effects such as variable suspension and flat tires.

Note

Vehicles and their wheels have several properties measured in real-world units (meters, centimeters, and newtons) with default values that produce realistic behavior for vehicles of size similar to an average automobile. If you design your scene on a different scale, proportionally change the values of these properties to fit the desired behavior of your app or game.

## Topics

### Creating a Wheel

convenience init(node: SCNNode)

Creates a wheel object.

### Managing a Wheel’s Connection to a Vehicle

var connectionPosition: SCNVector3

The position of the wheel’s connection to the vehicle’s chassis.

var axle: SCNVector3

The direction of the axis that the wheel spins around to move the vehicle.

var steeringAxis: SCNVector3

The direction of the axis that the wheel pivots around to steer the vehicle.

### Simulating Wheel Size

var radius: CGFloat

The radius of the wheel.

### Simulating Traction

var frictionSlip: CGFloat

The traction between the wheel and any surface in contact with it.

### Simulating Suspension

var suspensionStiffness: CGFloat

The spring coefficient of the suspension between the vehicle and the wheel.

var suspensionCompression: CGFloat

The coefficient that limits the speed of the suspension returning to its rest length when compressed.

var suspensionDamping: CGFloat

The damping ratio that limits oscillation in the vehicle’s suspension.

var maximumSuspensionTravel: CGFloat

The maximum distance that the wheel is allowed to move up or down relative to its connection point, in centimeters.

var maximumSuspensionForce: CGFloat

The maximum force of the suspension between the vehicle and the wheel, in newtons.

var suspensionRestLength: CGFloat

The resting length of the suspension, in meters.

### Inspecting the Wheel Node

var node: SCNNode

The node providing the wheel’s visual representation.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Vehicle Simulation

class SCNPhysicsVehicle

A physics behavior that modifies a physics body to behave like a car, motorcycle, or other wheeled vehicle.

