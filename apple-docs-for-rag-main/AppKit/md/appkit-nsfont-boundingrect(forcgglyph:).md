

- AppKit
- NSFont
-  boundingRect(forCGGlyph:) 

Instance Method

# boundingRect(forCGGlyph:)

Returns the bounding rectangle for the specified glyph, scaled to the receiver’s size.

macOS 10.13+

``` source
func boundingRect(forCGGlyph glyph: CGGlyph) -> NSRect
```

## Discussion

Japanese fonts encoded with the scheme “EUC12-NJE-CFEncoding” do not have individual metrics or bounding boxes available for the glyphs above 127. For those glyphs, this method returns the bounding rectangle for the font instead.

## See Also

### Getting Bounding Rectangles

var boundingRectForFont: NSRect

The font’s bounding rectangle, scaled to the font’s size.

func getBoundingRects(NSRectArray, forCGGlyphs: UnsafePointer&lt;CGGlyph>, count: Int)

Returns an array of the bounding rectangles for the specified glyphs rendered by the receiver.

