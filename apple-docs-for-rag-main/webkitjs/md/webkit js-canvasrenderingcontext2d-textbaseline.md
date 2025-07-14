

- WebKit JS
- CanvasRenderingContext2D
-  textBaseline 

Instance Property

# textBaseline

A string that specifies how the bounding box aligns vertically relative to the y-coordinate.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute DOMString textBaseline;
```

## Discussion

The y-coordinate of a line of text corresponds to the point on the text glyphs specified by `textBaseline`. Possible values are `top`, `hanging`, `middle`, `alphabetic` (default), `ideographic`, and `bottom`. The position of each value on the text glyphs is illustrated in Figure 1.

Figure 1 Text baseline values

See textBaseline Constants for descriptions of the constants.

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

textAlign

A string that specifies whether text is left-justified, right-justified, or centered.

