

- AppKit
- NSLayoutManager
-  insertGlyphs(\_:length:forStartingGlyphAt:characterIndex:) Deprecated

Instance Method

# insertGlyphs(\_:length:forStartingGlyphAt:characterIndex:)

Inserts the given glyphs into the glyph cache at the given index and maps them to characters beginning at the given character index.

macOS 10.0–10.11Deprecated

``` source
func insertGlyphs(
    _ glyphs: UnsafePointer,
    length: Int,
    forStartingGlyphAt glyphIndex: Int,
    characterIndex charIndex: Int
)
```

Deprecated

Use -setGlyphs:properties:characterIndexes:font:forGlyphRange instead

## Parameters 

`glyphs`  

The glyphs to insert.

`length`  

The number of glyphs to insert.

`glyphIndex`  

The index in the glyph cache to begin inserting glyphs.

`charIndex`  

Index of first character to be mapped.

## Discussion

This method is part of the `NSGlyphStorage` protocol, for use by the glyph generator. It enables bulk insertion of glyphs into the glyph cache.

## See Also

### Methods

func showCGGlyphs(UnsafePointer&lt;CGGlyph>, positions: UnsafePointer&lt;NSPoint>, count: Int, font: NSFont, matrix: AffineTransform, attributes: [NSAttributedString.Key : Any], in: NSGraphicsContext)

Renders the glyphs at the specified positions, using the specified attributes.

Deprecated

func invalidateGlyphs(onLayoutInvalidationForGlyphRange: NSRange)

Specifies explicitly when portions of the glyph stream depend on layout.

Deprecated

func invalidateLayout(forCharacterRange: NSRange, isSoft: Bool, actualCharacterRange: NSRangePointer?)

Invalidates the layout information for the glyphs mapped to the given range of characters.

Deprecated

func textStorage(NSTextStorage, edited: Int, range: NSRange, changeInLength: Int, invalidatedRange: NSRange)

Invalidates glyph and layout information for a portion of the text in the given text storage object.

Deprecated

func insertGlyph(NSGlyph, atGlyphIndex: Int, characterIndex: Int)

Inserts a single glyph into the glyph stream at the given index and maps it to the character at the given character index.

Deprecated

func glyph(at: Int) -> NSGlyph

Returns the glyph at the specified index.

Deprecated

func glyph(at: Int, isValidIndex: UnsafeMutablePointer&lt;ObjCBool>?) -> NSGlyph

Returns the glyph at a specified index, and optionally returns a flag indicating whether the requested index is valid.

Deprecated

func replaceGlyph(at: Int, withGlyph: NSGlyph)

Replaces the glyph at the given index with a new glyph.

Deprecated

func getGlyphs(UnsafeMutablePointer&lt;NSGlyph>?, range: NSRange) -> Int

Fills the passed-in buffer with a sequence of glyphs.

Deprecated

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;NSGlyph>?, characterIndexes: UnsafeMutablePointer&lt;Int>?, glyphInscriptions: UnsafeMutablePointer&lt;NSGlyphInscription>?, elasticBits: UnsafeMutablePointer&lt;ObjCBool>?) -> Int

Returns the glyphs and information needed to perform layout for the given glyph range.

Deprecated

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;NSGlyph>?, characterIndexes: UnsafeMutablePointer&lt;Int>?, glyphInscriptions: UnsafeMutablePointer&lt;NSGlyphInscription>?, elasticBits: UnsafeMutablePointer&lt;ObjCBool>?, bidiLevels: UnsafeMutablePointer&lt;UInt8>?) -> Int

Returns the glyphs and information needed to perform layout for the given glyph range.

Deprecated

func deleteGlyphs(in: NSRange)

Deletes the glyphs in the given range from the receiver’s glyph store.

Deprecated

func setCharacterIndex(Int, forGlyphAt: Int)

Sets the index of the character corresponding to the glyph at the given glyph index.

Deprecated

func intAttribute(Int, forGlyphAt: Int) -> Int

Returns the value of the attribute identified by the given attribute tag for the glyph at the given index.

Deprecated

func setIntAttribute(Int, value: Int, forGlyphAt: Int)

Sets a custom attribute value for a given glyph.

Deprecated

