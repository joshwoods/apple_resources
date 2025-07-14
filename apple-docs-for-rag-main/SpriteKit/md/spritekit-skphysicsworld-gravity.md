

- SpriteKit
- SKPhysicsWorld
-  gravity 

Instance Property

# gravity

A vector that specifies the gravitational acceleration applied to physics bodies in the physics world.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var gravity: CGVector { get set }
```

## Discussion

The components of this property are measured in meters per second. The default value is `(0.0,-9.8)`, which represent’s Earth’s gravity.

## See Also

### Configuring the Physics World

var speed: CGFloat

The rate at which the simulation executes.

