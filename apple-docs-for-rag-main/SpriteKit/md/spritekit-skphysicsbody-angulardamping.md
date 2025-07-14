

- SpriteKit
- SKPhysicsBody
-  angularDamping 

Instance Property

# angularDamping

A property that reduces the body’s rotational velocity.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var angularDamping: CGFloat { get set }
```

## Mentioned in 

Pinning and Rotating Physics Bodies

## Discussion

This property is used to simulate fluid or air friction forces on the body. The property must be a value between `0.0` and `1.0`. The default value is `0.1`. If the value is `0.0`, no angular damping is applied to the object.

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

var friction: CGFloat

The roughness of the surface of the physics body.

var restitution: CGFloat

The bounciness of the physics body.

var linearDamping: CGFloat

A property that reduces the body’s linear velocity.

