

- SpriteKit
- SKPhysicsJointPin
-  shouldEnableLimits 

Instance Property

# shouldEnableLimits

A Boolean value that indicates whether the pin joint’s rotation is limited to a specific range of values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var shouldEnableLimits: Bool { get set }
```

## Discussion

The default value is false. If true, the lowerAngleLimit and upperAngleLimit properties are used to limit the angle of the pin joint.

## See Also

### Configuring a Pin Joint

var rotationSpeed: CGFloat

The speed, in radians per second, at which the physics bodies are driven around the pin joint.

var lowerAngleLimit: CGFloat

The smallest angle allowed for the pin joint, in radians.

var upperAngleLimit: CGFloat

The largest angle allowed for the pin joint, in radians.

var frictionTorque: CGFloat

The resistance applied by the pin joint to spinning around the anchor point.

