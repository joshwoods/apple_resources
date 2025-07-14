

- AppKit
- NSFont
-  glyph(withName:) 

Instance Method

# glyph(withName:)

Returns the named encoded glyph, or –1 if the receiver contains no such glyph.

macOS

``` source
func glyph(withName name: String) -> NSGlyph
```

## Parameters 

`name`  

The name of the glyph.

## Return Value

The named encoded glyph.

## Discussion

Returns –1 if the glyph named `glyphName` isn’t encoded.

Glyph names in fonts do not always accurately identify the glyph. The layout manager, an instance of NSLayoutManager, finds the correspondence between characters and glyphs. See Text Layout Programming Guide and NSLayoutManager for more information.

## See Also

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

func screenFont(with: NSFontRenderingMode) -> NSFont

Returns a bitmapped screen font, when sent to a font object representing a scalable PostScript font, with the specified rendering mode, matching the receiver in typeface and matrix (or size), or `nil` if such a font can’t be found.

func withSize(CGFloat) -> NSFont

