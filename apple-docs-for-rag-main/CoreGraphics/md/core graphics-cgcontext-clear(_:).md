

- Core Graphics
- CGContext
-  clear(\_:) 

Instance Method

# clear(\_:)

Paints a transparent rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func clear(_ rect: CGRect)
```

## Parameters 

`rect`  

The rectangle, in user space coordinates.

## Discussion

If the provided context is a window or bitmap context, Core Graphics clears the rectangle. For other context types, Core Graphics fills the rectangle in a device-dependent manner. However, you should not use this function in contexts other than window or bitmap contexts.

## See Also

### Drawing Shapes

func fill(CGRect)

Paints the area contained within the provided rectangle, using the fill color in the current graphics state.

func fill([CGRect])

Paints the areas contained within the provided rectangles, using the fill color in the current graphics state.

func fillEllipse(in: CGRect)

Paints the area of the ellipse that fits inside the provided rectangle, using the fill color in the current graphics state.

func stroke(CGRect)

Paints a rectangular path.

func stroke(CGRect, width: CGFloat)

Paints a rectangular path, using the specified line width.

func strokeEllipse(in: CGRect)

Strokes an ellipse that fits inside the specified rectangle.

func strokeLineSegments(between: [CGPoint])

Strokes a sequence of line segments.

