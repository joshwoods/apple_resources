

- SpriteKit
- SKPhysicsBody
-  init(circleOfRadius:) 

Initializer

# init(circleOfRadius:)

Creates a circular physics body centered on the owning node’s origin.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(circleOfRadius r: CGFloat)
```

## Parameters 

`r`  

The radius of the circle.

## Return Value

A new volume-based physics body.

## Mentioned in 

Shaping a Physics Body to Match a Node’s Graphics

## Discussion

The following code shows the code that creates the physics body for a spherical or circular object. Because the physics body is attached to a sprite object, it usually needs volume. In this case, the sprite image is assumed to closely approximate a circle centered on the anchor point, so the radius of the circle is calculated and used to create the physics body.

Listing 1. A physics body for a circular sprite

- Swift
- Obj-C

```
let sprite = SKSpriteNode(imageNamed: "sphere.png")
sprite.physicsBody = SKPhysicsBody(circleOfRadius: sprite.size.width / 2)
sprite.physicsBody?.isDynamic = true
```

```
SKSpriteNode *sprite = [SKSpriteNode spriteNodeWithImageNamed:@"sphere.png"];
sprite.physicsBody = [SKPhysicsBody bodyWithCircleOfRadius:sprite.size.width/2];
sprite.physicsBody.dynamic = YES;
```

If the physics body were significantly smaller than the sprite’s image, the data used to create the physics body might need to be provided by some other source, such as a property list.

## See Also

### Creating a Body from a Shape

init(circleOfRadius: CGFloat, center: CGPoint)

Creates a circular physics body centered on an arbitrary point.

init(rectangleOf: CGSize)

Creates a rectangular physics body centered on the owning node’s origin.

init(rectangleOf: CGSize, center: CGPoint)

Creates a rectangular physics body centered on an arbitrary point.

init(polygonFrom: CGPath)

Creates a polygonal physics body.

