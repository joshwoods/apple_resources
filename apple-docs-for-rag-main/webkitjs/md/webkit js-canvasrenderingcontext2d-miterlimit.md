

- WebKit JS
- CanvasRenderingContext2D
-  miterLimit 

Instance Property

# miterLimit

A floating-point number that controls the miter limit ratio for mitered line joins.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
attribute unrestricted float miterLimit;
```

## Discussion

The `miterLimit` value must be a nonzero positive number. This property affects the appearance of line joins when the `lineJoin` property is set to `miter`.

The miter length is the distance from the point where the join occurs to the intersection of the line edges on the outside of the join. The miter limit ratio is the maximum allowed ratio of the miter length to half the line width. If the miter length would cause the miter limit ratio to be exceeded, the second triangle of the miter join is not rendered, and the join is beveled.

## See Also

### Filling and Stroking Lines and Paths

fill

Fills the current path using the current fill color, gradient, or pattern.

fillStyle

A CSS color, a gradient, or a pattern used to fill shapes and text.

lineCap

A string specifying the type of end cap to put on lines to be drawn using `lineTo()`.

lineJoin

A string specifying the manner in which line joins are drawn.

lineWidth

A floating-point number that controls the width of lines and strokes, in pixels.

stroke

Draws the outline of the current path using the current stroke style and line width.

strokeStyle

A CSS color, a gradient, or a pattern used to stroke lines and shapes.

