

- AppKit
- NSLayoutManager
-  getGlyphs(in:glyphs:characterIndexes:glyphInscriptions:elasticBits:bidiLevels:) Deprecated

Instance Method

# getGlyphs(in:glyphs:characterIndexes:glyphInscriptions:elasticBits:bidiLevels:)

Returns the glyphs and information needed to perform layout for the given glyph range.

macOS 10.0–10.11Deprecated

``` source
func getGlyphs(
    in glyphRange: NSRange,
    glyphs glyphBuffer: UnsafeMutablePointer?,
    characterIndexes charIndexBuffer: UnsafeMutablePointer?,
    glyphInscriptions inscribeBuffer: UnsafeMutablePointer?,
    elasticBits elasticBuffer: UnsafeMutablePointer?,
    bidiLevels bidiLevelBuffer: UnsafeMutablePointer?
) -> Int
```

Deprecated

Use -getGlyphsInRange:glyphs:properties:characterIndexes:bidiLevels: instead

## Parameters 

`glyphRange`  

The range of glyphs to lay out.

`glyphBuffer`  

On output, the sequence of glyphs needed to lay out the given glyph range.

`charIndexBuffer`  

On output, the indexes of the original characters corresponding to the given glyph range. Note that a glyph at index 1 is not necessarily mapped to the character at index 1, since a glyph may be for a ligature or accent.

`inscribeBuffer`  

On output, the inscription attributes for each glyph, which are used to lay out characters that are combined together. The possible values are described in `Constants`.

`elasticBuffer`  

On output, values indicating whether a glyph is elastic for each glyph. An elastic glyph can be made longer at the end of a line or when needed for justification.

`bidiLevelBuffer`  

On output, the direction of each glyph for bidirectional text. The values range from 0 to 61 as defined by Unicode Standard Annex \#9. An even value means the glyph goes left-to-right, and an odd value means the glyph goes right-to-left.

## Return Value

The number of glyphs returned in `glyphBuffer`.

## Discussion

This method and getGlyphs(in:glyphs:characterIndexes:glyphInscriptions:elasticBits:) are intended primarily to enable the typesetter to obtain in bulk the glyphs and other information that it needs to perform layout. These methods return all glyphs in the range, including `NSNullGlyph` and not-shown glyphs. They do not null-terminate the results. Each pointer passed in should either be `NULL`, or else point to sufficient memory to hold `glyphRange.length` elements.

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

func insertGlyphs(UnsafePointer&lt;NSGlyph>, length: Int, forStartingGlyphAt: Int, characterIndex: Int)

Inserts the given glyphs into the glyph cache at the given index and maps them to characters beginning at the given character index.

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

