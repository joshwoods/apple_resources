

- WebKit JS
- CanvasRenderingContext2D
-  fill 

Instance Method

# fill

Fills the current path using the current fill color, gradient, or pattern.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
void fill(
    DOMPath path, 
    optional CanvasWindingRule winding
);
```

## Discussion

The `fill()` method makes a solid shape from the current path, even if the path is not closed. For complex paths, it is possible to create a filled shape with a unfilled areas. For example, to create a doughnut, rather than a circle, create a circular subpath, going clockwise or or counterclockwise, then create another circular subpath, completely inside the first circle or completely surrounding it, with the second circle going in the opposite direction clockwise from the first circle. The area between the two circles is filled, but the interior of the smaller circle is not. The `fill()` method uses the **non-zero number winding rule** to determine whether a point within a path should be filled or not.

## See Also

### Filling and Stroking Lines and Paths

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

strokeStyle

A CSS color, a gradient, or a pattern used to stroke lines and shapes.

