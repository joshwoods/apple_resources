

- AppKit
- Fonts
- NSFont
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Methods

func getAdvancements(NSSizeArray, forGlyphs: UnsafePointer&lt;NSGlyph>, count: Int)

Returns an array of the advancements for the specified glyphs rendered by the receiver.

Deprecated

func getAdvancements(NSSizeArray, forPackedGlyphs: UnsafeRawPointer, length: Int)

Returns an array of the advancements for the specified packed glyphs and rendered by the receiver.

Deprecated

func advancement(forGlyph: NSGlyph) -> NSSize

Returns the nominal spacing for the given glyph—the distance the current point moves after showing the glyph—accounting for the receiver’s size.

Deprecated

func boundingRect(forGlyph: NSGlyph) -> NSRect

Returns the bounding rectangle for the specified glyph, scaled to the receiver’s size.

Deprecated

func getBoundingRects(NSRectArray, forGlyphs: UnsafePointer&lt;NSGlyph>, count: Int)

Returns an array of the bounding rectangles for the specified glyphs rendered by the receiver.

Deprecated

func glyph(withName: String) -> NSGlyph

Returns the named encoded glyph, or –1 if the receiver contains no such glyph.

func screenFont(with: NSFontRenderingMode) -> NSFont

Returns a bitmapped screen font, when sent to a font object representing a scalable PostScript font, with the specified rendering mode, matching the receiver in typeface and matrix (or size), or `nil` if such a font can’t be found.

### Properties

var renderingMode: NSFontRenderingMode

The rendering mode of the font.

var printer: NSFont

The scalable PostScript font corresponding to current font.

var screen: NSFont

The bitmapped screen font for the current font.

### Types

enum NSMultibyteGlyphPacking

A constant for glyph packing.

Deprecated

enum NSFontRenderingMode

The font rendering mode.

