

- SceneKit
- SCNPhysicsVehicleWheel
-  suspensionRestLength 

Instance Property

# suspensionRestLength

The resting length of the suspension, in meters.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var suspensionRestLength: CGFloat { get set }
```

## Discussion

This property measures the length of the simulated spring between the vehicle and its wheel when the spring is not stressed by the weight of either body. When the wheel receives a shock (for example, when the vehicle runs over a bump), SceneKit adds the difference between the wheel’s current position and its connection position to this rest length and then applies a force between the wheel and vehicle proportional to the total.

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

var maximumSuspensionForce: CGFloat

The maximum force of the suspension between the vehicle and the wheel, in newtons.

