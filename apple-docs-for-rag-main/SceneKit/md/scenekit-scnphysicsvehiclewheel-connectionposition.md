

- SceneKit
- SCNPhysicsVehicleWheel
-  connectionPosition 

Instance Property

# connectionPosition

The position of the wheel’s connection to the vehicle’s chassis.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var connectionPosition: SCNVector3 { get set }
```

## Discussion

This vector is expressed in the coordinate space of the node containing the vehicle’s chassis. When you create a wheel from a node, SceneKit uses the node’s position property as the wheel’s connection point.

## See Also

### Managing a Wheel’s Connection to a Vehicle

var axle: SCNVector3

The direction of the axis that the wheel spins around to move the vehicle.

var steeringAxis: SCNVector3

The direction of the axis that the wheel pivots around to steer the vehicle.

