

- SceneKit
- SCNPhysicsVehicleWheel
-  suspensionCompression 

Instance Property

# suspensionCompression

The coefficient that limits the speed of the suspension returning to its rest length when compressed.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var suspensionCompression: CGFloat { get set }
```

## Discussion

The default suspension coefficient is `4.4`. Lower values cause the wheel to return to its natural position more quickly.

## See Also

### Simulating Suspension

var suspensionStiffness: CGFloat

The spring coefficient of the suspension between the vehicle and the wheel.

var suspensionDamping: CGFloat

The damping ratio that limits oscillation in the vehicle’s suspension.

var maximumSuspensionTravel: CGFloat

The maximum distance that the wheel is allowed to move up or down relative to its connection point, in centimeters.

var maximumSuspensionForce: CGFloat

The maximum force of the suspension between the vehicle and the wheel, in newtons.

var suspensionRestLength: CGFloat

The resting length of the suspension, in meters.

