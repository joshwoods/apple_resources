

- Core Graphics
- CGContext
-  clip(using:) 

Instance Method

# clip(using:)

Modifies the current clipping path.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func clip(using rule: CGPathFillRule = .winding)
```

## Parameters 

`rule`  

The rule for determining which areas to treat as the interior of the path. See CGPathFillRule.

This parameter defaults to the CGPathFillRule.winding rule if unspecified.

## Discussion

A clipping path restricts the paintable area: painting operations take effect only for those areas in the interior of the clipping path. This method uses the specified rule to calculate the intersection of the current path with the current clipping path. The path resulting from the intersection is used as the new current clipping path for subsequent painting operations.

If the current path contains any non-closed subpaths, this method treats each subpath as if it had been closed with the closePath() method, then applies the specified rule to determine which areas to fill.

After determining the new clipping path, this method clears the context’s current path.

Unlike the current path, the current clipping path is part of the graphics state. Therefore, to re-enlarge the paintable area by restoring the clipping path to a prior state, you must save the graphics state before you clip and restore the graphics state after you’ve completed any clipped drawing.

## See Also

### Working with the Current Clipping Path

func clip(to: CGRect)

Sets the clipping path to the intersection of the current clipping path with the area defined by the specified rectangle.

func clip(to: [CGRect])

Sets the clipping path to the intersection of the current clipping path with the region defined by an array of rectangles.

func clip(to: CGRect, mask: CGImage)

Maps a mask into the specified rectangle and intersects it with the current clipping area of the graphics context.

var boundingBoxOfClipPath: CGRect

Returns the bounding box of a clipping path.

