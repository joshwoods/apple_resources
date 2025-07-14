

- SceneKit
- SCNPhysicsVehicleWheel
-  axle 

Instance Property

# axle

The direction of the axis that the wheel spins around to move the vehicle.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var axle: SCNVector3 { get set }
```

## Discussion

This vector is expressed in the coordinate space of the node containing the vehicle’s chassis. The default axle direction is `{-1.0, 0.0, 0.0}`.

## See Also

### Managing a Wheel’s Connection to a Vehicle

var connectionPosition: SCNVector3

The position of the wheel’s connection to the vehicle’s chassis.

var steeringAxis: SCNVector3

The direction of the axis that the wheel pivots around to steer the vehicle.

