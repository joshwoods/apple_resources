

- AppKit
- NSGradient
-  draw(fromCenter:radius:toCenter:radius:options:) 

Instance Method

# draw(fromCenter:radius:toCenter:radius:options:)

Draws a radial gradient between the specified circles.

macOS 10.5+

``` source
func draw(
    fromCenter startCenter: NSPoint,
    radius startRadius: CGFloat,
    toCenter endCenter: NSPoint,
    radius endRadius: CGFloat,
    options: NSGradient.DrawingOptions = []
)
```

## Parameters 

`startCenter`  

The center point of the circle that represents the beginning of the gradient.

`startRadius`  

The radius of the circle that represents the beginning of the gradient.

`endCenter`  

The center point of the circle that represents the end of the gradient.

`endRadius`  

The radius of the circle that represents the end of the gradient.

`options`  

The gradient options, if any. You can use these options to extend the gradient size beyond the start and end circles. For more information, see NSGradient.DrawingOptions.

## Discussion

This method draws a radial gradient pattern starting at the first circle and ending at the second circle. The gradient color transitions occur in circular bands emanating from the starting circle and ending at the second circle.

This is a primitive method used by the `NSGradient` class to draw radial gradients. Because this method does not perform any clipping of the gradient fill pattern, you must ensure that the clipping region is configured properly if you intend to invoke this method directly. By default, the clipping region is set to the current view or window in which drawing occurs.

## See Also

### Drawing a Radial Gradient

func draw(in: NSRect, relativeCenterPosition: NSPoint)

Draws a radial gradient starting at the center of the specified rectangle.

func draw(in: NSBezierPath, relativeCenterPosition: NSPoint)

Draws a radial gradient starting at the center point of the specified path.

