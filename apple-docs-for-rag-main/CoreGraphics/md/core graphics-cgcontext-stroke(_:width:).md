

- Core Graphics
- CGContext
-  stroke(\_:width:) 

Instance Method

# stroke(\_:width:)

Paints a rectangular path, using the specified line width.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func stroke(
    _ rect: CGRect,
    width: CGFloat
)
```

## Parameters 

`rect`  

A rectangle, in user space coordinates.

`width`  

A value, in user space units, that is greater than zero. This value does not affect the line width values in the current graphics state.

## Discussion

Aside from the line width value, Core Graphics uses the current attributes of the graphics state (such as stroke color) to paint the line. The line straddles the path, with half of the total width on either side.

The current path is cleared as a side effect of calling this function.

## See Also

### Drawing Shapes

func clear(CGRect)

Paints a transparent rectangle.

func fill(CGRect)

Paints the area contained within the provided rectangle, using the fill color in the current graphics state.

func fill([CGRect])

Paints the areas contained within the provided rectangles, using the fill color in the current graphics state.

func fillEllipse(in: CGRect)

Paints the area of the ellipse that fits inside the provided rectangle, using the fill color in the current graphics state.

func stroke(CGRect)

Paints a rectangular path.

func strokeEllipse(in: CGRect)

Strokes an ellipse that fits inside the specified rectangle.

func strokeLineSegments(between: [CGPoint])

Strokes a sequence of line segments.

