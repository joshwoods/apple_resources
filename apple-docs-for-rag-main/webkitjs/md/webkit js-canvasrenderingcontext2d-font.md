

- WebKit JS
- CanvasRenderingContext2D
-  font 

Instance Property

# font

A string containing font settings, such as the font family, size, and weight.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute DOMString font;
```

## Discussion

Set this property to a string specifying all the font properties you wish to set, just as you would the CSS `font` property. Note that you must use the combined (all-in-one) font settings string. Setting individual font properties such as `font-size` is not supported.

## See Also

### Drawing Text

fillText

Draws a line of text at the specified x,y coordinates, optionally scaled to a specified maximum width.

measureText

Determines the width of the bounding box required to render the specified text with the current font settings.

strokeText

Draws a line of text in outline at the specified x,y coordinates, optionally limited to a specified maximum width.

textAlign

A string that specifies whether text is left-justified, right-justified, or centered.

textBaseline

A string that specifies how the bounding box aligns vertically relative to the y-coordinate.

