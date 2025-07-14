

- SpriteKit
- SKPhysicsBody
-  area 

Instance Property

# area

The area covered by the body.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var area: CGFloat { get }
```

## Mentioned in 

Configuring a Physics Body

## Discussion

This property is used in conjunction with the density property to calculate the body’s mass.

The value returned for the area is measured in meters: if you need to convert it into points — as used by SpriteKit — multiply the values by 150². The following listing shows how to calculate the area of a box which is ten points square.

```
let bodySize = CGSize(width: 10, height: 10)
let physicsBody = SKPhysicsBody(rectangleOf: bodySize)
let areaInPoints = physicsBody.area * pow(150, 2) // areaInPoints = 100
```

## See Also

### Defining a Physics Body’s Physical Properties

Configuring a Physics Body

Move a physics body, and make it collide with other objects, by setting its physical properties once or changing them dynamically.

var mass: CGFloat

The mass of the body, in kilograms.

var density: CGFloat

The density of the object, in kilograms per square meter.

var friction: CGFloat

The roughness of the surface of the physics body.

var restitution: CGFloat

The bounciness of the physics body.

var linearDamping: CGFloat

A property that reduces the body’s linear velocity.

var angularDamping: CGFloat

A property that reduces the body’s rotational velocity.

