

- AppKit
- NSGradient
-  draw(in:angle:) 

Instance Method

# draw(in:angle:)

Fills the specified path with a linear gradient.

macOS 10.5+

``` source
func draw(
    in path: NSBezierPath,
    angle: CGFloat
)
```

## Parameters 

`path`  

The path object to fill.

`angle`  

The angle of the linear gradient, specified in degrees. Positive values indicate rotation in the counter-clockwise direction relative to the horizontal axis.

## Discussion

This convenience method behaves in a similar way to the draw(in:angle:) method, with the path object replacing the rectangle as the clipping region. Like the other method, the start and end colors are guaranteed to be visible at the farthest ends of the path.

The gradient formed by this method is clipped to `path`.

## See Also

### Drawing a Linear Gradient

func draw(from: NSPoint, to: NSPoint, options: NSGradient.DrawingOptions)

Draws a linear gradient between the specified start and end points.

func draw(in: NSRect, angle: CGFloat)

Fills the specified rectangle with a linear gradient.

