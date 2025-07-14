

- SpriteKit
- SKPhysicsWorld
-  speed 

Instance Property

# speed

The rate at which the simulation executes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var speed: CGFloat { get set }
```

## Discussion

The default value is `1.0`, which means the simulation runs at normal speed. A value other than the default changes the rate at which time passes in the physics simulation. For example, a speed value of `2.0` indicates that time in the physics simulation passes twice as fast as the scene’s simulation time. A value of `0.0` pauses the physics simulation.

## See Also

### Configuring the Physics World

var gravity: CGVector

A vector that specifies the gravitational acceleration applied to physics bodies in the physics world.

