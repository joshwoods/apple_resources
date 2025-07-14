

- AppKit
- NSFont
-  screenFont(with:) 

Instance Method

# screenFont(with:)

Returns a bitmapped screen font, when sent to a font object representing a scalable PostScript font, with the specified rendering mode, matching the receiver in typeface and matrix (or size), or `nil` if such a font can’t be found.

macOS

``` source
func screenFont(with renderingMode: NSFontRenderingMode) -> NSFont
```

## Discussion

For valid rendering modes, see NSFontRenderingMode.

Screen fonts are for direct use with the window server only. Never use them with Application Kit objects, such as in `setFont:` methods. Internally, the Application Kit automatically uses the corresponding screen font for a font object as long as the view is not rotated or scaled.

## See Also

### Related Documentation

var screen: NSFont

The bitmapped screen font for the current font.

var printer: NSFont

The scalable PostScript font corresponding to current font.

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

func getAdvancements(NSSizeArray, forPackedGlyphs: UnsafeRawPointer, length: Int)

Returns an array of the advancements for the specified packed glyphs and rendered by the receiver.

Deprecated

func getBoundingRects(NSRectArray, forGlyphs: UnsafePointer&lt;NSGlyph>, count: Int)

Returns an array of the bounding rectangles for the specified glyphs rendered by the receiver.

Deprecated

func glyph(withName: String) -> NSGlyph

Returns the named encoded glyph, or –1 if the receiver contains no such glyph.

func withSize(CGFloat) -> NSFont

