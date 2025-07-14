

- AppKit
- NSFont
-  getAdvancements(\_:forPackedGlyphs:length:) Deprecated

Instance Method

# getAdvancements(\_:forPackedGlyphs:length:)

Returns an array of the advancements for the specified packed glyphs and rendered by the receiver.

macOS

``` source
func getAdvancements(
    _ advancements: NSSizeArray,
    forPackedGlyphs packedGlyphs: UnsafeRawPointer,
    length: Int
)
```

Deprecated

Use getAdvancements(_:forCGGlyphs:count:) instead.

## Discussion

Returns in `advancements` an array of the advancements for the packed glyphs specified by `packedGlyphs` and rendered by the receiver. The `glyphCount` must specify the count of glyphs passed in `packedGlyphs`.

## See Also

### Related Documentation

var boundingRectForFont: NSRect

The font’s bounding rectangle, scaled to the font’s size.

### Instance Methods

func advancement(forGlyph: NSGlyph) -> NSSize

Returns the nominal spacing for the given glyph—the distance the current point moves after showing the glyph—accounting for the receiver’s size.

Deprecated

func boundingRect(forGlyph: NSGlyph) -> NSRect

Returns the bounding rectangle for the specified glyph, scaled to the receiver’s size.

Deprecated

func getAdvancements(NSSizeArray, forGlyphs: UnsafePointer&lt;NSGlyph>, count: Int)

Returns an array of the advancements for the specified glyphs rendered by the receiver.

Deprecated

func getBoundingRects(NSRectArray, forGlyphs: UnsafePointer&lt;NSGlyph>, count: Int)

Returns an array of the bounding rectangles for the specified glyphs rendered by the receiver.

Deprecated

func glyph(withName: String) -> NSGlyph

Returns the named encoded glyph, or –1 if the receiver contains no such glyph.

func screenFont(with: NSFontRenderingMode) -> NSFont

Returns a bitmapped screen font, when sent to a font object representing a scalable PostScript font, with the specified rendering mode, matching the receiver in typeface and matrix (or size), or `nil` if such a font can’t be found.

func withSize(CGFloat) -> NSFont

