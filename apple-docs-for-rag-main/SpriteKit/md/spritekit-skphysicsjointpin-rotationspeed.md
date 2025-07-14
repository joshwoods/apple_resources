

- SpriteKit
- SKPhysicsJointPin
-  rotationSpeed 

Instance Property

# rotationSpeed

The speed, in radians per second, at which the physics bodies are driven around the pin joint.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rotationSpeed: CGFloat { get set }
```

## Discussion

The frictionTorque property limits the maximum amount of torque that can be applied to the physics bodies.

## See Also

### Configuring a Pin Joint

var shouldEnableLimits: Bool

A Boolean value that indicates whether the pin joint’s rotation is limited to a specific range of values.

var lowerAngleLimit: CGFloat

The smallest angle allowed for the pin joint, in radians.

var upperAngleLimit: CGFloat

The largest angle allowed for the pin joint, in radians.

var frictionTorque: CGFloat

The resistance applied by the pin joint to spinning around the anchor point.

