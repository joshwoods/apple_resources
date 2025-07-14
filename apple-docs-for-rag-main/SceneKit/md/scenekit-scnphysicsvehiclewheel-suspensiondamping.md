

- SceneKit
- SCNPhysicsVehicleWheel
-  suspensionDamping 

Instance Property

# suspensionDamping

The damping ratio that limits oscillation in the vehicle’s suspension.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var suspensionDamping: CGFloat { get set }
```

## Discussion

*Damping ratio* measures the tendency of the suspension to oscillate after a shock—in other words, for the vehicle to bounce up and down after running over a bump. The default damping ratio of `2.3` causes the wheel to return to its neutral position quickly after a shock. Values lower than `1.0` result in more oscillation.

## See Also

### Simulating Suspension

var suspensionStiffness: CGFloat

The spring coefficient of the suspension between the vehicle and the wheel.

var suspensionCompression: CGFloat

The coefficient that limits the speed of the suspension returning to its rest length when compressed.

var maximumSuspensionTravel: CGFloat

The maximum distance that the wheel is allowed to move up or down relative to its connection point, in centimeters.

var maximumSuspensionForce: CGFloat

The maximum force of the suspension between the vehicle and the wheel, in newtons.

var suspensionRestLength: CGFloat

The resting length of the suspension, in meters.

