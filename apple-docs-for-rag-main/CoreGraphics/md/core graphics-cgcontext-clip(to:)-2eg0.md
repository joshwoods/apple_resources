

- Core Graphics
- CGContext
-  clip(to:) 

Instance Method

# clip(to:)

Sets the clipping path to the intersection of the current clipping path with the region defined by an array of rectangles.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func clip(to rects: [CGRect])
```

## Parameters 

`rects`  

An array of rectangles, in user space coordinates.

## Discussion

This method sets the clipping path to the intersection of the current clipping path and the region within the specified rectangles.

After determining the new clipping path, the function resets the context’s current path to an empty path.

## See Also

### Working with the Current Clipping Path

func clip(using: CGPathFillRule)

Modifies the current clipping path.

func clip(to: CGRect)

Sets the clipping path to the intersection of the current clipping path with the area defined by the specified rectangle.

func clip(to: CGRect, mask: CGImage)

Maps a mask into the specified rectangle and intersects it with the current clipping area of the graphics context.

var boundingBoxOfClipPath: CGRect

Returns the bounding box of a clipping path.

