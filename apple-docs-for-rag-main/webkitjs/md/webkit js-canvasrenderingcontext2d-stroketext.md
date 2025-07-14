

- WebKit JS
- CanvasRenderingContext2D
-  strokeText 

Instance Method

# strokeText

Draws a line of text in outline at the specified x,y coordinates, optionally limited to a specified maximum width.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
void strokeText(
    DOMString text, 
    unrestricted float x, 
    unrestricted float y, 
    optional unrestricted float maxWidth
);
```

## Parameters 

`text`  

A string containing the text to draw.

`x`  

The x-coordinate of the `textAlign` point (the left edge, right edge, or center of the text).

`y`  

The y-coordinate of the `textBaseline` point.

`maxWidth`  

The maximum width of the string, in pixels. This parameter is optional. If omitted, the string is drawn in the current font style; any text falling outside the canvas clipping region is clipped. If this parameter is provided, and the text would exceed the specified width, the text is scaled down until it fits within the specified width.

## Discussion

The `x`, `y`, and `maxWidth` parameter values are in the canvas’s current coordinate system, subject to the current transformation matrix (rotation, scale, and so on).

## See Also

### Drawing Text

fillText

Draws a line of text at the specified x,y coordinates, optionally scaled to a specified maximum width.

font

A string containing font settings, such as the font family, size, and weight.

measureText

Determines the width of the bounding box required to render the specified text with the current font settings.

textAlign

A string that specifies whether text is left-justified, right-justified, or centered.

textBaseline

A string that specifies how the bounding box aligns vertically relative to the y-coordinate.

