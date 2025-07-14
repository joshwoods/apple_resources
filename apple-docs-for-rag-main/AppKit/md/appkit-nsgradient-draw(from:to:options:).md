

- AppKit
- NSGradient
-  draw(from:to:options:) 

Instance Method

# draw(from:to:options:)

Draws a linear gradient between the specified start and end points.

macOS 10.5+

``` source
func draw(
    from startingPoint: NSPoint,
    to endingPoint: NSPoint,
    options: NSGradient.DrawingOptions = []
)
```

## Parameters 

`startingPoint`  

The starting point for the gradient, in the local coordinate system. The gradient’s first color is drawn at this point.

`endingPoint`  

The end point for the gradient, in the local coordinate system. The gradient’s last color is drawn at this point.

`options`  

The gradient options, if any. You can use these options to extend the gradient size beyond the start and end points. For more information, see `Gradient Drawing Options`.

## Discussion

This method draws the gradient color changes along the line formed by the two points. The gradient fill extends perpendicularly outward from line until it reaches the edges of the current clipping region.

This is a primitive method used by the `NSGradient` class to draw linear gradients. Because this method does not perform any clipping of the gradient fill pattern, you must ensure that the clipping region is configured properly if you intend to invoke this method directly. By default, the clipping region is set to the current view or window in which drawing occurs.

## See Also

### Drawing a Linear Gradient

func draw(in: NSRect, angle: CGFloat)

Fills the specified rectangle with a linear gradient.

func draw(in: NSBezierPath, angle: CGFloat)

Fills the specified path with a linear gradient.

