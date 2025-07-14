

- Core Graphics
- CGContext
-  strokeLineSegments(between:) 

Instance Method

# strokeLineSegments(between:)

Strokes a sequence of line segments.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func strokeLineSegments(between points: [CGPoint])
```

## Parameters 

`points`  

An array of points, organized as pairs—the starting point of a line segment followed by the ending point of a line segment. For example, the first point in the array specifies the starting position of the first line, the second point specifies the ending position of the first line, the third point specifies the starting position of the second line, and so forth.

## Discussion

This function creates a new path, adds the individual line segments to the path, and then strokes the path. The current path is cleared as a side effect of calling this function.

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

func stroke(CGRect, width: CGFloat)

Paints a rectangular path, using the specified line width.

func strokeEllipse(in: CGRect)

Strokes an ellipse that fits inside the specified rectangle.

