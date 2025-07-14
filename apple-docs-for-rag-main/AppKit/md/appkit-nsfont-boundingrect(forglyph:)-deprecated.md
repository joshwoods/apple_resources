

- AppKit
- NSFont
-  boundingRect(forGlyph:) Deprecated

Instance Method

# boundingRect(forGlyph:)

Returns the bounding rectangle for the specified glyph, scaled to the receiver’s size.

macOS

``` source
func boundingRect(forGlyph glyph: NSGlyph) -> NSRect
```

Deprecated

Use boundingRect(forCGGlyph:) instead.

## Discussion

Japanese fonts encoded with the scheme “EUC12-NJE-CFEncoding” do not have individual metrics or bounding boxes available for the glyphs above 127. For those glyphs, this method returns the bounding rectangle for the font instead.

## See Also

### Related Documentation

var boundingRectForFont: NSRect

The font’s bounding rectangle, scaled to the font’s size.

### Instance Methods

func advancement(forGlyph: NSGlyph) -> NSSize

Returns the nominal spacing for the given glyph—the distance the current point moves after showing the glyph—accounting for the receiver’s size.

Deprecated

func getAdvancements(NSSizeArray, forGlyphs: UnsafePointer&lt;NSGlyph>, count: Int)

Returns an array of the advancements for the specified glyphs rendered by the receiver.

Deprecated

func getAdvancements(NSSizeArray, forPackedGlyphs: UnsafeRawPointer, length: Int)

Returns an array of the advancements for the specified packed glyphs and rendered by the receiver.

Deprecated

func getBoundingRects(NSRectArray, forGlyphs: UnsafePointer&lt;NSGlyph>, count: Int)

Returns an array of the bounding rectangles for the specified glyphs rendered by the receiver.

Deprecated

func glyph(withName: String) -> NSGlyph

Returns the named encoded glyph, or –1 if the receiver contains no such glyph.

func screenFont(with: NSFontRenderingMode) -> NSFont

Returns a bitmapped screen font, when sent to a font object representing a scalable PostScript font, with the specified rendering mode, matching the receiver in typeface and matrix (or size), or `nil` if such a font can’t be found.

func withSize(CGFloat) -> NSFont

