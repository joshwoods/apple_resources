

- Core Graphics
- CGContext
-  fillEllipse(in:) 

Instance Method

# fillEllipse(in:)

Paints the area of the ellipse that fits inside the provided rectangle, using the fill color in the current graphics state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func fillEllipse(in rect: CGRect)
```

## Parameters 

`rect`  

A rectangle that defines the area for the ellipse to fit in.

## Discussion

The current path is cleared as a side effect of calling this function.

## See Also

### Drawing Shapes

func clear(CGRect)

Paints a transparent rectangle.

func fill(CGRect)

Paints the area contained within the provided rectangle, using the fill color in the current graphics state.

func fill([CGRect])

Paints the areas contained within the provided rectangles, using the fill color in the current graphics state.

func stroke(CGRect)

Paints a rectangular path.

func stroke(CGRect, width: CGFloat)

Paints a rectangular path, using the specified line width.

func strokeEllipse(in: CGRect)

Strokes an ellipse that fits inside the specified rectangle.

func strokeLineSegments(between: [CGPoint])

Strokes a sequence of line segments.

