

- AppKit
- NSFont
-  boundingRectForFont 

Instance Property

# boundingRectForFont

The font’s bounding rectangle, scaled to the font’s size.

macOS

``` source
var boundingRectForFont: NSRect { get }
```

## Discussion

The bounding rectangle is the union of the bounding rectangles of every glyph in the font.

## See Also

### Related Documentation

func boundingRect(forGlyph: NSGlyph) -> NSRect

Returns the bounding rectangle for the specified glyph, scaled to the receiver’s size.

Deprecated

### Getting Bounding Rectangles

func boundingRect(forCGGlyph: CGGlyph) -> NSRect

Returns the bounding rectangle for the specified glyph, scaled to the receiver’s size.

func getBoundingRects(NSRectArray, forCGGlyphs: UnsafePointer&lt;CGGlyph>, count: Int)

Returns an array of the bounding rectangles for the specified glyphs rendered by the receiver.

