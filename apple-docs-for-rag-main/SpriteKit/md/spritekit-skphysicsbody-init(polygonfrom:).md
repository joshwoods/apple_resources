

- SpriteKit
- SKPhysicsBody
-  init(polygonFrom:) 

Initializer

# init(polygonFrom:)

Creates a polygonal physics body.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(polygonFrom path: CGPath)
```

## Parameters 

`path`  

A convex polygonal path with counterclockwise winding and no self intersections. The points are specified relative to the owning node’s origin.

## Return Value

A new volume-based physics body.

## Mentioned in 

Shaping a Physics Body to Match a Node’s Graphics

## See Also

### Creating a Body from a Shape

init(circleOfRadius: CGFloat)

Creates a circular physics body centered on the owning node’s origin.

init(circleOfRadius: CGFloat, center: CGPoint)

Creates a circular physics body centered on an arbitrary point.

init(rectangleOf: CGSize)

Creates a rectangular physics body centered on the owning node’s origin.

init(rectangleOf: CGSize, center: CGPoint)

Creates a rectangular physics body centered on an arbitrary point.

