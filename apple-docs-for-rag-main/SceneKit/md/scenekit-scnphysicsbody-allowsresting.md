

- SceneKit
- SCNPhysicsBody
-  allowsResting 

Instance Property

# allowsResting

A Boolean value that specifies whether SceneKit can automatically mark the physics body at rest.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var allowsResting: Bool { get set }
```

## Discussion

If true (the default), SceneKit keeps track of whether the body is moving or affected by forces, automatically setting its isResting property to true when it is “at rest.” The physics simulation runs faster when simulating fewer bodies, so treating a body as resting temporarily removes it from the simulation to improve performance.

SceneKit automatically returns a resting body to the simulation if another body collides with it, if you change its position or velocity, or if you apply a force to it. However, SceneKit uses a faster, less accurate simulation when deciding whether to change a body’s isResting property back to false. If testing your app reveals unexpected physics behaviors involving resting bodies, changing those bodies’ allowsResting property to false may improve simulation accuracy.

## See Also

### Defining When a Body Can Move

var isResting: Bool

A Boolean value that indicates whether the physics body is at rest.

func setResting(Bool)

Tells SceneKit whether to treat the body as currently being in motion.

