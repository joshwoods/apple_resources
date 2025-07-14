

- SpriteKit
- SKPhysicsJointPin
-  upperAngleLimit 

Instance Property

# upperAngleLimit

The largest angle allowed for the pin joint, in radians.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var upperAngleLimit: CGFloat { get set }
```

## Mentioned in 

Pinning and Rotating Physics Bodies

## Discussion

The default value is `0.0`.

## See Also

### Configuring a Pin Joint

var rotationSpeed: CGFloat

The speed, in radians per second, at which the physics bodies are driven around the pin joint.

var shouldEnableLimits: Bool

A Boolean value that indicates whether the pin joint’s rotation is limited to a specific range of values.

var lowerAngleLimit: CGFloat

The smallest angle allowed for the pin joint, in radians.

var frictionTorque: CGFloat

The resistance applied by the pin joint to spinning around the anchor point.

