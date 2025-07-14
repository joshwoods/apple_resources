

- UIKit
- TextKit
- NSLayoutManager
-  Deprecated symbols 

API Collection

# Deprecated symbols

Review unsupported symbols and their replacements.

## Topics

### Methods

func showCGGlyphs(UnsafePointer&lt;CGGlyph>, positions: UnsafePointer&lt;CGPoint>, count: Int, font: UIFont, matrix: CGAffineTransform, attributes: [NSAttributedString.Key : Any], in: CGContext)

Renders the glyphs at the specified positions, using the specified attributes.

Deprecated

func invalidateGlyphs(onLayoutInvalidationForGlyphRange glyphRange: NSRange)

Specifies explicitly when portions of the glyph stream depend on layout.

Deprecated

func invalidateLayout(forCharacterRange charRange: NSRange, isSoft flag: Bool, actualCharacterRange actualCharRange: NSRangePointer?)

Invalidates the layout information for the glyphs mapped to the given range of characters.

Deprecated

func textStorage(_ str: NSTextStorage, edited editedMask: Int = [], range newCharRange: NSRange, changeInLength delta: Int, invalidatedRange invalidatedCharRange: NSRange)

Invalidates glyph and layout information for a portion of the text in the given text storage object.

Deprecated

func insertGlyph(_ glyph: NSGlyph, atGlyphIndex glyphIndex: Int, characterIndex charIndex: Int)

Inserts a single glyph into the glyph stream at the given index and maps it to the character at the given character index.

Deprecated

func insertGlyphs(_ glyphs: UnsafePointer&lt;NSGlyph>, length: Int, forStartingGlyphAt glyphIndex: Int, characterIndex charIndex: Int)

Inserts the given glyphs into the glyph cache at the given index and maps them to characters beginning at the given character index.

Deprecated

func glyph(at: Int) -> CGGlyph

Returns the glyph at the specified index.

Deprecated

func glyph(at: Int, isValidIndex: UnsafeMutablePointer&lt;ObjCBool>?) -> CGGlyph

Returns the glyph at a specified index, and optionally returns a flag indicating whether the requested index is valid.

Deprecated

func replaceGlyph(at glyphIndex: Int, withGlyph newGlyph: NSGlyph)

Replaces the glyph at the given index with a new glyph.

Deprecated

func getGlyphs(_ glyphArray: UnsafeMutablePointer&lt;NSGlyph>?, range glyphRange: NSRange) -> Int

Fills the passed-in buffer with a sequence of glyphs.

Deprecated

func getGlyphs(in glyphRange: NSRange, glyphs glyphBuffer: UnsafeMutablePointer&lt;NSGlyph>?, characterIndexes charIndexBuffer: UnsafeMutablePointer&lt;Int>?, glyphInscriptions inscribeBuffer: UnsafeMutablePointer&lt;NSGlyphInscription>?, elasticBits elasticBuffer: UnsafeMutablePointer&lt;ObjCBool>?) -> Int

Returns the glyphs and information needed to perform layout for the given glyph range.

Deprecated

func getGlyphs(in glyphRange: NSRange, glyphs glyphBuffer: UnsafeMutablePointer&lt;NSGlyph>?, characterIndexes charIndexBuffer: UnsafeMutablePointer&lt;Int>?, glyphInscriptions inscribeBuffer: UnsafeMutablePointer&lt;NSGlyphInscription>?, elasticBits elasticBuffer: UnsafeMutablePointer&lt;ObjCBool>?, bidiLevels bidiLevelBuffer: UnsafeMutablePointer&lt;UInt8>?) -> Int

Returns the glyphs and information needed to perform layout for the given glyph range.

Deprecated

func deleteGlyphs(in glyphRange: NSRange)

Deletes the glyphs in the given range from the receiver’s glyph store.

Deprecated

func setCharacterIndex(_ charIndex: Int, forGlyphAt glyphIndex: Int)

Sets the index of the character corresponding to the glyph at the given glyph index.

Deprecated

func intAttribute(_ attributeTag: Int, forGlyphAt glyphIndex: Int) -> Int

Returns the value of the attribute identified by the given attribute tag for the glyph at the given index.

Deprecated

func setIntAttribute(_ attributeTag: Int, value val: Int, forGlyphAt glyphIndex: Int)

Sets a custom attribute value for a given glyph.

Deprecated

func setLocations(_ locations: NSPointArray, startingGlyphIndexes glyphIndexes: UnsafeMutablePointer&lt;Int>, count: Int, forGlyphRange glyphRange: NSRange)

Sets locations for many glyph ranges at once.

Deprecated

func rectArray(forCharacterRange charRange: NSRange, withinSelectedCharacterRange selCharRange: NSRange, in container: NSTextContainer, rectCount: UnsafeMutablePointer&lt;Int>) -> NSRectArray?

Returns an array of rectangles and, by reference, the number of such rectangles, that define the region in the given container enclosing the given character range.

func rectArray(forGlyphRange glyphRange: NSRange, withinSelectedGlyphRange selGlyphRange: NSRange, in container: NSTextContainer, rectCount: UnsafeMutablePointer&lt;Int>) -> NSRectArray?

Returns an array of rectangles and, by reference, the number of such rectangles, that define the region in the given container enclosing the given glyph range.

func substituteFont(for originalFont: NSFont) -> NSFont

Replaces the specified font with a suitable screen font if one is available.

Deprecated

### Properties

var hyphenationFactor: CGFloat

The threshold controlling when hyphenation is done.

Deprecated

attributedString

The text storage object from which the `NSGlyphGenerator` object procures characters for glyph generation.

layoutOptions

The layout manager’s current layout options.

var usesScreenFonts: Bool { get set }

A Boolean that controls using screen fonts to calculate layout and display text.

Deprecated

### Types

Glyph Attributes

Attributes that are used only inside the glyph generation machinery, but must also be shared between components.

