

- AppKit
- NSLayoutManager
-  rectArray(forCharacterRange:withinSelectedCharacterRange:in:rectCount:) 

Instance Method

# rectArray(forCharacterRange:withinSelectedCharacterRange:in:rectCount:)

Returns an array of rectangles and, by reference, the number of such rectangles, that define the region in the given container enclosing the given character range.

macOS

``` source
func rectArray(
    forCharacterRange charRange: NSRange,
    withinSelectedCharacterRange selCharRange: NSRange,
    in container: NSTextContainer,
    rectCount: UnsafeMutablePointer
) -> NSRectArray?
```

## Parameters 

`charRange`  

The character range for which to return rectangles.

`selCharRange`  

Selected characters within `charRange`, which can affect the size of the rectangles; it must be equal to or contain `charRange`. If the caller is interested in this more from an enclosing point of view rather than a selection point of view, pass `{NSNotFound, 0}` as the selected range.

`container`  

The text container in which the text is laid out.

`rectCount`  

The number of rectangles returned.

## Return Value

The array of rectangles enclosing the given range.

## Discussion

These rectangles can be used to draw the text background or highlight for the given range of characters. If a selected range is given in `selCharRange`, the rectangles returned are correct for drawing the selection. Selection rectangles are generally more complicated than enclosing rectangles and supplying a selected range is the clue this method uses to determine whether to go to the trouble of doing this special work.

This method will do the minimum amount of work required to answer the question. The resulting array is owned by the layout manager and will be reused when this method, rectArray(forGlyphRange:withinSelectedGlyphRange:in:rectCount:), or boundingRect(forGlyphRange:in:) is called. One of these methods may be called indirectly. If you aren’t going to use the rectangles right away, you should copy them to another location. These rectangles are always in container coordinates.

The number of rectangles returned isn’t necessarily the number of lines enclosing the specified range. Contiguous lines can share an enclosing rectangle, and lines broken into several fragments have a separate enclosing rectangle for each fragment.

These rectangles don’t necessarily enclose glyphs that draw outside their line fragment rectangles; use boundingRect(forGlyphRange:in:) to determine the area that contains all drawing performed for a range of glyphs.

Performs glyph generation and layout if needed.

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

