

- WebKit JS
- CanvasRenderingContext2D
-  lineWidth 

Instance Property

# lineWidth

A floating-point number that controls the width of lines and strokes, in pixels.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
attribute unrestricted float lineWidth;
```

## Discussion

The default line width is 1 pixel. This property specifies not only the width of lines drawn with `lineTo()`, but also the stroke thickness of any `stroke()` operation.

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

miterLimit

A floating-point number that controls the miter limit ratio for mitered line joins.

stroke

Draws the outline of the current path using the current stroke style and line width.

strokeStyle

A CSS color, a gradient, or a pattern used to stroke lines and shapes.

