

- AppKit
- NSTextFinderClient
-  drawCharacters(in:forContentView:) 

Instance Method

# drawCharacters(in:forContentView:)

Draw the glyphs for the requested character range as they are drawn in the given content view.

macOS

``` source
optional func drawCharacters(
    in range: NSRange,
    forContentView view: NSView
)
```

## Parameters 

`range`  

The character range.

`view`  

The content view.

## Discussion

If the character range partially intersects a glyph range, then the full glyph is drawn to avoid additional layout.

The given range is guaranteed to be completely contained by the given view. When this method is called, a drawing context effectively identical to the one provided to the view’s draw(_:) method is configured. This method is mainly used to draw find indicator contents, so implementations should check -the view property isDrawingFindIndicator to ensure that the text will be easily readable against the background of the find indicator when it returns true. If this method is not implemented, then the find indicator will be drawn using the content view’s draw(_:) method instead.

