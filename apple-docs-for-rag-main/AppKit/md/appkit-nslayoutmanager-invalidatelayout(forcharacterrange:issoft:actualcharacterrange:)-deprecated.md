

- AppKit
- NSLayoutManager
-  invalidateLayout(forCharacterRange:isSoft:actualCharacterRange:) Deprecated

Instance Method

# invalidateLayout(forCharacterRange:isSoft:actualCharacterRange:)

Invalidates the layout information for the glyphs mapped to the given range of characters.

macOS 10.0–10.11Deprecated

``` source
func invalidateLayout(
    forCharacterRange charRange: NSRange,
    isSoft flag: Bool,
    actualCharacterRange actualCharRange: NSRangePointer?
)
```

Deprecated

Use -invalidateLayoutForCharacterRange:actualCharacterRange: instead

## Parameters 

`charRange`  

The character range for which glyphs are invalidated.

`flag`  

If true, invalidates internal caches in the layout manager; if false, invalidates layout. See the discussion section.

`actualCharRange`  

If not `NULL`, on output, the range of characters mapped to the glyphs whose layout information is invalidated. This range can be larger than the range of characters given due to the effect of context on glyphs and layout.

## Discussion

This method only invalidates information; it performs no glyph generation or layout. You should rarely need to invoke this method.

For code that needs to work on both OS X v10.5 and previous releases, the following procedures should be used. For OS X v10.4 and before, invalidation should consist of

1.  Calling this method with the `flag` set to true, for the range that has actually become invalid.

2.  Calling this method with the `flag` set to false, for the range (if any) that follows that range, usually extending to the end of the text, that might need to be moved due to relayout of the invalidated range.

As of OS X v10.5, the semantics of the `flag` parameter are slightly different. Soft layout holes are obsolete in macOS 10.5 and later, so the flag is no longer necessary. If the method is called with `flag` set to false, then it has the effect of invalidating layout. If it’s called with the `flag` set to true, then it does not actually invalidate layout; it invalidates a number of internal caches, but otherwise has no effect, and in general is unnecessary.

This method is superseded by invalidateLayout(forCharacterRange:actualCharacterRange:) and will be deprecated in a future release.

## See Also

### Methods

func showCGGlyphs(UnsafePointer&lt;CGGlyph>, positions: UnsafePointer&lt;NSPoint>, count: Int, font: NSFont, matrix: AffineTransform, attributes: [NSAttributedString.Key : Any], in: NSGraphicsContext)

Renders the glyphs at the specified positions, using the specified attributes.

Deprecated

func invalidateGlyphs(onLayoutInvalidationForGlyphRange: NSRange)

Specifies explicitly when portions of the glyph stream depend on layout.

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

func setIntAttribute(Int, value: Int, forGlyphAt: Int)

Sets a custom attribute value for a given glyph.

Deprecated

