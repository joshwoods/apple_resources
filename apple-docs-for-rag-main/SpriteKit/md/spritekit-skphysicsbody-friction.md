

- SpriteKit
- SKPhysicsBody
-  friction 

Instance Property

# friction

The roughness of the surface of the physics body.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var friction: CGFloat { get set }
```

## Discussion

This property is used to apply a frictional force to physics bodies in contact with this physics body. The property must be a value between `0.0` and `1.0`. The default value is `0.2`.

## See Also

### Defining a Physics Body’s Physical Properties

Configuring a Physics Body

Move a physics body, and make it collide with other objects, by setting its physical properties once or changing them dynamically.

var mass: CGFloat

The mass of the body, in kilograms.

var density: CGFloat

The density of the object, in kilograms per square meter.

var area: CGFloat

The area covered by the body.

var restitution: CGFloat

The bounciness of the physics body.

var linearDamping: CGFloat

A property that reduces the body’s linear velocity.

var angularDamping: CGFloat

A property that reduces the body’s rotational velocity.

