

- UIKit
- NSLayoutManager
-  glyph(at:) Deprecated

Instance Method

# glyph(at:)

Returns the glyph at the specified index.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
func glyph(at glyphIndex: Int) -> CGGlyph
```

Deprecated

Use cgGlyph(at:) instead.

## Parameters 

`glyphIndex`  

The index of a glyph in the receiver. This value must not exceed the bounds of the receiver’s glyph array.

## Return Value

The glyph at `glyphIndex`.

## Discussion

Raises an `NSRangeException` if `glyphIndex` is out of bounds.

Performs glyph generation if needed. To avoid an exception with glyph(at:) you must first check the glyph index against the number of glyphs, which requires generating all glyphs. Another method, glyph(at:isValidIndex:), generates glyphs only up to the one requested, so using it can be more efficient.

## See Also

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

