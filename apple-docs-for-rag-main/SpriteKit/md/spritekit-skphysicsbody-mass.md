

- SpriteKit
- SKPhysicsBody
-  mass 

Instance Property

# mass

The mass of the body, in kilograms.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var mass: CGFloat { get set }
```

## Mentioned in 

Configuring a Physics Body

## Discussion

The actual unit is arbitrary as long as relative masses of objects are consistent throughout the game. The mass of the body affects its momentum as well as how forces are applied to the object.

The mass and density properties are interrelated. When you change the value of either property, the other property’s value is automatically recalculated to be consistent. The default value is based on the size of the physics body and the body’s default density.

## See Also

### Defining a Physics Body’s Physical Properties

Configuring a Physics Body

Move a physics body, and make it collide with other objects, by setting its physical properties once or changing them dynamically.

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

var angularDamping: CGFloat

A property that reduces the body’s rotational velocity.

