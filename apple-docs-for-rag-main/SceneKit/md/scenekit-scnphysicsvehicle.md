

- SceneKit
-  SCNPhysicsVehicle 

Class

# SCNPhysicsVehicle

A physics behavior that modifies a physics body to behave like a car, motorcycle, or other wheeled vehicle.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsVehicle
```

## Overview

To build a vehicle, designate an SCNPhysicsBody object as its chassis and an array of SCNPhysicsVehicleWheel objects as its wheels. For each wheel, you define physical characteristics such as suspension and traction, and associate a node in your scene to provide the wheel’s size and visual representation. After you construct a vehicle, you can control it in terms of acceleration, braking, and steering.

Although it’s also possible to use a set of physics bodies and joints to collectively simulate a wheeled vehicle, the SCNPhysicsVehicle class implements a higher-level simulation that provides realistic vehicle behavior with more efficient simulation performance.

## Topics

### Creating a Vehicle

convenience init(chassisBody: SCNPhysicsBody, wheels: [SCNPhysicsVehicleWheel])

Creates a vehicle behavior.

### Working with a Vehicle’s Physical Characteristics

var chassisBody: SCNPhysicsBody

The physics body representing the vehicle’s chassis.

var wheels: [SCNPhysicsVehicleWheel]

An array of SCNPhysicsVehicleWheel objects representing the vehicle’s wheels.

### Driving a Vehicle

func applyEngineForce(CGFloat, forWheelAt: Int)

Applies a force between the specified wheel and the ground under the vehicle.

func applyBrakingForce(CGFloat, forWheelAt: Int)

Applies a force between the specified wheel and the ground under the vehicle.

func setSteeringAngle(CGFloat, forWheelAt: Int)

Pivots the specified wheel around its steering axis.

var speedInKilometersPerHour: CGFloat

The vehicle’s ground speed, in kilometers per hour.

## Relationships

### Inherits From

- SCNPhysicsBehavior

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

### Vehicle Simulation

class SCNPhysicsVehicleWheel

The appearance and physical characteristics of an individual wheel associated with an physics vehicle behavior.

