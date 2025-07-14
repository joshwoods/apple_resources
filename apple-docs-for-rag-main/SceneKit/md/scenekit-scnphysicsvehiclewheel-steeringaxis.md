

- SceneKit
- SCNPhysicsVehicleWheel
-  steeringAxis 

Instance Property

# steeringAxis

The direction of the axis that the wheel pivots around to steer the vehicle.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var steeringAxis: SCNVector3 { get set }
```

## Discussion

This vector is expressed in the coordinate space of the node containing the vehicle’s chassis. The default steering axis is `{0.0, -1.0, 0.0}`.

When you steer a wheel using the vehicle’s setSteeringAngle(_:forWheelAt:) method, the wheel pivots relative to this axis. For example, you can implement a vehicle whose rear wheels steer opposite its front wheels by reversing this vector’s direction for the rear wheels and then applying the same steering angle to all wheels.

## See Also

### Managing a Wheel’s Connection to a Vehicle

var connectionPosition: SCNVector3

The position of the wheel’s connection to the vehicle’s chassis.

var axle: SCNVector3

The direction of the axis that the wheel spins around to move the vehicle.

