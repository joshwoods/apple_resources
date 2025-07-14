

- SpriteKit
- SKPhysicsBody
-  init(circleOfRadius:center:) 

Initializer

# init(circleOfRadius:center:)

Creates a circular physics body centered on an arbitrary point.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    circleOfRadius r: CGFloat,
    center: CGPoint
)
```

## Parameters 

`r`  

The radius of the circle.

`center`  

The origin of the circle in the owning node’s coordinate system.

## Return Value

A new volume-based physics body.

## See Also

### Creating a Body from a Shape

init(circleOfRadius: CGFloat)

Creates a circular physics body centered on the owning node’s origin.

init(rectangleOf: CGSize)

Creates a rectangular physics body centered on the owning node’s origin.

init(rectangleOf: CGSize, center: CGPoint)

Creates a rectangular physics body centered on an arbitrary point.

init(polygonFrom: CGPath)

Creates a polygonal physics body.

