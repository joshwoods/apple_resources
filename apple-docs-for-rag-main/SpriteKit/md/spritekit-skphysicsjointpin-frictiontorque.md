

- SpriteKit
- SKPhysicsJointPin
-  frictionTorque 

Instance Property

# frictionTorque

The resistance applied by the pin joint to spinning around the anchor point.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var frictionTorque: CGFloat { get set }
```

## Mentioned in 

Pinning and Rotating Physics Bodies

## Discussion

The range of values is from `0.0` to `1.0`. The default value is `0.0`. If a value greater than the default is specified, friction is applied to reduce the object’s angular velocity around the pin.

## See Also

### Configuring a Pin Joint

var rotationSpeed: CGFloat

The speed, in radians per second, at which the physics bodies are driven around the pin joint.

var shouldEnableLimits: Bool

A Boolean value that indicates whether the pin joint’s rotation is limited to a specific range of values.

var lowerAngleLimit: CGFloat

The smallest angle allowed for the pin joint, in radians.

var upperAngleLimit: CGFloat

The largest angle allowed for the pin joint, in radians.

