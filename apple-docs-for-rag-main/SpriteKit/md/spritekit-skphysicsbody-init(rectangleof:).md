

- SpriteKit
- SKPhysicsBody
-  init(rectangleOf:) 

Initializer

# init(rectangleOf:)

Creates a rectangular physics body centered on the owning node’s origin.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(rectangleOf s: CGSize)
```

## Parameters 

`s`  

The size of the rectangle.

## Return Value

A new volume-based physics body.

## See Also

### Creating a Body from a Shape

init(circleOfRadius: CGFloat)

Creates a circular physics body centered on the owning node’s origin.

init(circleOfRadius: CGFloat, center: CGPoint)

Creates a circular physics body centered on an arbitrary point.

init(rectangleOf: CGSize, center: CGPoint)

Creates a rectangular physics body centered on an arbitrary point.

init(polygonFrom: CGPath)

Creates a polygonal physics body.

