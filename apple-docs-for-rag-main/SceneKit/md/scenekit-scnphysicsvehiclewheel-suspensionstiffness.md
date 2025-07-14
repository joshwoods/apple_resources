

- SceneKit
- SCNPhysicsVehicleWheel
-  suspensionStiffness 

Instance Property

# suspensionStiffness

The spring coefficient of the suspension between the vehicle and the wheel.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var suspensionStiffness: CGFloat { get set }
```

## Discussion

The spring coefficient determines both how quickly the wheel returns to its natural position after a shock (for example, when the vehicle runs over a bump) and how much force from the shock it transmits to the vehicle. The default spring coefficient is `2.0`.

## See Also

### Simulating Suspension

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

