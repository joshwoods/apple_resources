

- SceneKit
- SCNPhysicsBody
-  isResting 

Instance Property

# isResting

A Boolean value that indicates whether the physics body is at rest.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isResting: Bool { get }
```

## Discussion

This property’s default value is false, but SceneKit’s physics simulation may automatically set it to true if the body is not moving and not affected by any forces. A resting body does not participate in the simulation until another body collides with it or you change its position or velocity or apply a force to it.

## See Also

### Defining When a Body Can Move

var allowsResting: Bool

A Boolean value that specifies whether SceneKit can automatically mark the physics body at rest.

func setResting(Bool)

Tells SceneKit whether to treat the body as currently being in motion.

