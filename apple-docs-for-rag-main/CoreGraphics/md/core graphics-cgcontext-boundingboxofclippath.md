

- Core Graphics
- CGContext
-  boundingBoxOfClipPath 

Instance Property

# boundingBoxOfClipPath

Returns the bounding box of a clipping path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var boundingBoxOfClipPath: CGRect { get }
```

## Discussion

The bounding box is the smallest rectangle completely enclosing all points in the clipping path, including control points for any Bezier curves in the path.

## See Also

### Working with the Current Clipping Path

func clip(using: CGPathFillRule)

Modifies the current clipping path.

func clip(to: CGRect)

Sets the clipping path to the intersection of the current clipping path with the area defined by the specified rectangle.

func clip(to: [CGRect])

Sets the clipping path to the intersection of the current clipping path with the region defined by an array of rectangles.

func clip(to: CGRect, mask: CGImage)

Maps a mask into the specified rectangle and intersects it with the current clipping area of the graphics context.

