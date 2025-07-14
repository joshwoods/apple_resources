

- WebKit JS
- CanvasRenderingContext2D
-  strokeStyle 

Instance Property

# strokeStyle

A CSS color, a gradient, or a pattern used to stroke lines and shapes.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
attribute custom strokeStyle;
```

## Discussion

This property may be set to any CSS color, to a pattern object, or to a linear or radial gradient object. When the `stroke()`, `strokeRect()`, or `strokeText()` operation is performed, the lines are drawn using the style specified by `strokeStyle`.

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

miterLimit

A floating-point number that controls the miter limit ratio for mitered line joins.

stroke

Draws the outline of the current path using the current stroke style and line width.

### Related Documentation

createRadialGradient

Creates a radial gradient object using the cone defined by the specified starting and ending circles.

createLinearGradient

Creates a linear gradient object with a specified start point and a specified end point.

createPattern

Creates a pattern object using the specified image as a template. The pattern can be specified as repeating horizontally, vertically, both horizontally and vertically (the default), or not at all.

