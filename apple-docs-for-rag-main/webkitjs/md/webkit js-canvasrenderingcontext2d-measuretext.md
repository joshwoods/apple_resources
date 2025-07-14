

- WebKit JS
- CanvasRenderingContext2D
-  measureText 

Instance Method

# measureText

Determines the width of the bounding box required to render the specified text with the current font settings.

Safari Desktop 4.0+Safari Mobile 3.0+

``` source
TextMetrics measureText(
    DOMString text
);
```

## Parameters 

`text`  

A string containing the text to measure.

## Return Value

An object whose `width` property contains the width in pixels of the bounding box needed to render the text without clipping.

## Discussion

Use this method to determine how much space is needed to render a string, or to measure the width of an existing string.

## See Also

### Drawing Text

fillText

Draws a line of text at the specified x,y coordinates, optionally scaled to a specified maximum width.

font

A string containing font settings, such as the font family, size, and weight.

strokeText

Draws a line of text in outline at the specified x,y coordinates, optionally limited to a specified maximum width.

textAlign

A string that specifies whether text is left-justified, right-justified, or centered.

textBaseline

A string that specifies how the bounding box aligns vertically relative to the y-coordinate.

