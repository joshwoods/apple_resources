

- Core Graphics
- CGContext
-  clip(to:) 

Instance Method

# clip(to:)

Sets the clipping path to the intersection of the current clipping path with the area defined by the specified rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func clip(to rect: CGRect)
```

## Parameters 

`rect`  

The location and dimensions of the rectangle, in user space, to be used in determining the new clipping path.

## Discussion

This function sets the specified graphics context’s clipping region to the area which intersects both the current clipping path and the specified rectangle.

After determining the new clipping path, the function resets the context’s current path to an empty path.

## See Also

### Working with the Current Clipping Path

func clip(using: CGPathFillRule)

Modifies the current clipping path.

func clip(to: [CGRect])

Sets the clipping path to the intersection of the current clipping path with the region defined by an array of rectangles.

func clip(to: CGRect, mask: CGImage)

Maps a mask into the specified rectangle and intersects it with the current clipping area of the graphics context.

var boundingBoxOfClipPath: CGRect

Returns the bounding box of a clipping path.

