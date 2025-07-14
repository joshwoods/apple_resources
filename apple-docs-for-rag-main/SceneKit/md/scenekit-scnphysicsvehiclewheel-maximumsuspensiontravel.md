

- SceneKit
- SCNPhysicsVehicleWheel
-  maximumSuspensionTravel 

Instance Property

# maximumSuspensionTravel

The maximum distance that the wheel is allowed to move up or down relative to its connection point, in centimeters.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var maximumSuspensionTravel: CGFloat { get set }
```

## Discussion

*Travel* is the total distance a wheel is allowed to move (in both directions), in the coordinate system of the node containing the vehicle’s chassis. The default suspension travel is `500.0`.

## See Also

### Simulating Suspension

var suspensionStiffness: CGFloat

The spring coefficient of the suspension between the vehicle and the wheel.

var suspensionCompression: CGFloat

The coefficient that limits the speed of the suspension returning to its rest length when compressed.

var suspensionDamping: CGFloat

The damping ratio that limits oscillation in the vehicle’s suspension.

var maximumSuspensionForce: CGFloat

The maximum force of the suspension between the vehicle and the wheel, in newtons.

var suspensionRestLength: CGFloat

The resting length of the suspension, in meters.

