

- AppKit
- NSGradient
-  draw(in:relativeCenterPosition:) 

Instance Method

# draw(in:relativeCenterPosition:)

Draws a radial gradient starting at the center point of the specified path.

macOS 10.5+

``` source
func draw(
    in path: NSBezierPath,
    relativeCenterPosition: NSPoint
)
```

## Parameters 

`path`  

The path to fill.

`relativeCenterPosition`  

The relative location within the bounding rectangle of `path` to use as the center point of the gradient’s end circle. Each coordinate must contain a value between -1.0 and 1.0. A coordinate value of 0 represents the center of the path’s bounding rectangle along the given axis. In the default coordinate system, a value of -1.0 corresponds to the bottom or left edge of the bounding rectangle and a value of 1.0 corresponds to the top or right edge.

## Discussion

The center point of the starting circle is the same as the center point of `path`. The radius of the starting circle is 0, resulting in the starting circle being just a point.

The center point of the end circle starts at the center point of `path` and is modified by the value in the `relativeCenterPosition` parameter. For example, if `relativeCenterPosition` contains the point (1.0, 1.0), the center of the end circle is located in the top-right corner of the path’s bounding rectangle. The radius of the end circle is set to the smallest value that ensures `rect` is covered by the end circle.

The gradient formed by this method is clipped to `path`.

## See Also

### Drawing a Radial Gradient

func draw(fromCenter: NSPoint, radius: CGFloat, toCenter: NSPoint, radius: CGFloat, options: NSGradient.DrawingOptions)

Draws a radial gradient between the specified circles.

func draw(in: NSRect, relativeCenterPosition: NSPoint)

Draws a radial gradient starting at the center of the specified rectangle.

