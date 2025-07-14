

- SceneKit
- SCNPhysicsVehicleWheel
-  maximumSuspensionForce 

Instance Property

# maximumSuspensionForce

The maximum force of the suspension between the vehicle and the wheel, in newtons.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var maximumSuspensionForce: CGFloat { get set }
```

## Discussion

The physics simulation applies a force of no greater than this magnitude when contact with the ground causes the wheel to move relative to the vehicle. The default maximum suspension force is `6000.0`.

## See Also

### Simulating Suspension

var suspensionStiffness: CGFloat

The spring coefficient of the suspension between the vehicle and the wheel.

var suspensionCompression: CGFloat

The coefficient that limits the speed of the suspension returning to its rest length when compressed.

var suspensionDamping: CGFloat

The damping ratio that limits oscillation in the vehicle’s suspension.

var maximumSuspensionTravel: CGFloat

The maximum distance that the wheel is allowed to move up or down relative to its connection point, in centimeters.

var suspensionRestLength: CGFloat

The resting length of the suspension, in meters.

