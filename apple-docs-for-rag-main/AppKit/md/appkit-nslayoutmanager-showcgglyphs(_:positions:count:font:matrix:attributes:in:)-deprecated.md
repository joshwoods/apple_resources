

- AppKit
- NSLayoutManager
-  showCGGlyphs(\_:positions:count:font:matrix:attributes:in:) Deprecated

Instance Method

# showCGGlyphs(\_:positions:count:font:matrix:attributes:in:)

Renders the glyphs at the specified positions, using the specified attributes.

macOS 10.7–10.15Deprecated

``` source
func showCGGlyphs(
    _ glyphs: UnsafePointer,
    positions: UnsafePointer,
    count glyphCount: Int,
    font: NSFont,
    matrix textMatrix: AffineTransform,
    attributes: [NSAttributedString.Key : Any] = [:],
    in graphicsContext: NSGraphicsContext
)
```

Deprecated

Use showCGGlyphs(_:positions:count:font:textMatrix:attributes:in:) instead.

## Parameters 

`glyphs`  

The glyphs to draw; may contain embedded `NULL` bytes.

`positions`  

The positions at which to draw the glyphs in the user space coordinate system.

`glyphCount`  

The number of glyphs.

`font`  

The font applied to the graphics state. This value can be different from the `NSFontAttributeName` value in the `attributes` argument because of various font substitutions that the system automatically executes.

`textMatrix`  

The affine transform mapping the text space coordinate system to the user space coordinate system. The `tx` and `ty` components of `textMatrix` are ignored since Quartz overrides them with the glyph positions.

`attributes`  

A dictionary of glyph attributes. See Glyph Attributes for supported keys and values.

`graphicsContext`  

If non-`nil`, `graphicsContext` is already configured according to the text attributes arguments: `font`, `textMatrix`, and `attributes`.

## Discussion

`NSLayoutManager` invokes this primitive method unless an override implementation of the deprecated showPackedGlyphs:length:glyphRange:atPoint:font:color:printingAdjustment: method exists and this method is not overridden.

## See Also

### Methods

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

func setIntAttribute(Int, value: Int, forGlyphAt: Int)

Sets a custom attribute value for a given glyph.

Deprecated

