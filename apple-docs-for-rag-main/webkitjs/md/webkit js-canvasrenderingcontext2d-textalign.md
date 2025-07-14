

- WebKit JS
- CanvasRenderingContext2D
-  textAlign 

Instance Property

# textAlign

A string that specifies whether text is left-justified, right-justified, or centered.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute DOMString textAlign;
```

## Discussion

Possible values are `start` (default), `end`, `left`, `right`, and `center`. The values `start` and `end` are equivalent to either `left` or `right`, depending on the text direction.

## See Also

### Drawing Text

fillText

Draws a line of text at the specified x,y coordinates, optionally scaled to a specified maximum width.

font

A string containing font settings, such as the font family, size, and weight.

measureText

Determines the width of the bounding box required to render the specified text with the current font settings.

strokeText

Draws a line of text in outline at the specified x,y coordinates, optionally limited to a specified maximum width.

textBaseline

A string that specifies how the bounding box aligns vertically relative to the y-coordinate.

