

- AppKit
- NSFont
-  getBoundingRects(\_:forCGGlyphs:count:) 

Instance Method

# getBoundingRects(\_:forCGGlyphs:count:)

Returns an array of the bounding rectangles for the specified glyphs rendered by the receiver.

macOS 10.13+

``` source
func getBoundingRects(
    _ bounds: NSRectArray,
    forCGGlyphs glyphs: UnsafePointer,
    count glyphCount: Int
)
```

## Discussion

Returns in `bounds` an array of the bounding rectangles for the glyphs specified by `glyphs` and rendered by the receiver. The `glyphCount` value must specify the count of glyphs passed in `glyphs`.

## See Also

### Getting Bounding Rectangles

var boundingRectForFont: NSRect

The font’s bounding rectangle, scaled to the font’s size.

func boundingRect(forCGGlyph: CGGlyph) -> NSRect

Returns the bounding rectangle for the specified glyph, scaled to the receiver’s size.

