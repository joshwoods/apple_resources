

- WebKit JS
- CanvasRenderingContext2D
-  fillStyle 

Instance Property

# fillStyle

A CSS color, a gradient, or a pattern used to fill shapes and text.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
attribute custom fillStyle;
```

## Discussion

This property can be set to any CSS color—for example “red”, rgb(255,0,0), \#ff0000, or rgba(255,0,0,1). This property can also be set to a gradient object or a pattern object.

## See Also

### Filling and Stroking Lines and Paths

fill

Fills the current path using the current fill color, gradient, or pattern.

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

strokeStyle

A CSS color, a gradient, or a pattern used to stroke lines and shapes.

### Related Documentation

createRadialGradient

Creates a radial gradient object using the cone defined by the specified starting and ending circles.

createLinearGradient

Creates a linear gradient object with a specified start point and a specified end point.

createPattern

Creates a pattern object using the specified image as a template. The pattern can be specified as repeating horizontally, vertically, both horizontally and vertically (the default), or not at all.

