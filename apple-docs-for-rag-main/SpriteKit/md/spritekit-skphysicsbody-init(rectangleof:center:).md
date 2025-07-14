

- SpriteKit
- SKPhysicsBody
-  init(rectangleOf:center:) 

Initializer

# init(rectangleOf:center:)

Creates a rectangular physics body centered on an arbitrary point.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    rectangleOf s: CGSize,
    center: CGPoint
)
```

## Parameters 

`s`  

The size of the rectangle.

`center`  

The center of the square in the owning node’s coordinate system.

## Return Value

A new volume-based physics body.

## See Also

### Creating a Body from a Shape

init(circleOfRadius: CGFloat)

Creates a circular physics body centered on the owning node’s origin.

init(circleOfRadius: CGFloat, center: CGPoint)

Creates a circular physics body centered on an arbitrary point.

init(rectangleOf: CGSize)

Creates a rectangular physics body centered on the owning node’s origin.

init(polygonFrom: CGPath)

Creates a polygonal physics body.

