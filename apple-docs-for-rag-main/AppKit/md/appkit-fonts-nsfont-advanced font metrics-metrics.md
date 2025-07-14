

- AppKit
- Fonts
- NSFont
-  Advanced Font Metrics 

API Collection

# Advanced Font Metrics

Retrieve details about ascender and descender heights, glyph bounding rectangles, glyph advancements, and more.

## Topics

### Getting the Font Metrics

var ascender: CGFloat

The top y-coordinate, offset from the baseline, of the font’s longest ascender.

var descender: CGFloat

The bottom y-coordinate, offset from the baseline, of the font’s longest descender.

var capHeight: CGFloat

The cap height of the font.

var leading: CGFloat

The leading value of the font.

var xHeight: CGFloat

The x-height of the font.

### Getting Underline and Italic Metrics

var italicAngle: CGFloat

The number of degrees that the font is slanted counterclockwise from the vertical.

var underlinePosition: CGFloat

The baseline offset to use when drawing underlines with the font.

var underlineThickness: CGFloat

The thickness to use when drawing underlines with the font.

### Getting Bounding Rectangles

var boundingRectForFont: NSRect

The font’s bounding rectangle, scaled to the font’s size.

func boundingRect(forCGGlyph: CGGlyph) -> NSRect

Returns the bounding rectangle for the specified glyph, scaled to the receiver’s size.

func getBoundingRects(NSRectArray, forCGGlyphs: UnsafePointer&lt;CGGlyph>, count: Int)

Returns an array of the bounding rectangles for the specified glyphs rendered by the receiver.

### Getting Glyph Advancements

var maximumAdvancement: NSSize

The maximum advance of any of the font’s glyphs.

func advancement(forCGGlyph: CGGlyph) -> NSSize

Returns the nominal spacing for the given glyph—the distance the current point moves after showing the glyph—accounting for the receiver’s size.

func getAdvancements(NSSizeArray, forCGGlyphs: UnsafePointer&lt;CGGlyph>, count: Int)

Returns an array of the advancements for the specified glyphs rendered by the receiver.

### Getting the Font Matrices

var matrix: UnsafePointer&lt;CGFloat>

The transformation matrix associated with the font.

var textTransform: AffineTransform

The current transformation matrix of the font.

class var identityMatrix: UnsafePointer&lt;CGFloat>

The identify matrix for the font.

## See Also

### Getting Font Metrics and Information

var pointSize: CGFloat

The point size of the font.

var coveredCharacterSet: CharacterSet

The character set containing all of the nominal characters that the font can render.

var fontDescriptor: NSFontDescriptor

The font descriptor object for the font.

var isFixedPitch: Bool

A Boolean value indicating whether all glyphs in the font have the same advancement.

var mostCompatibleStringEncoding: UInt

The string encoding that works best with the font.

