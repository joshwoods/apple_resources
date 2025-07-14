

- UIKit
- NSLayoutManager
-  showCGGlyphs(\_:positions:count:font:matrix:attributes:in:) Deprecated

Instance Method

# showCGGlyphs(\_:positions:count:font:matrix:attributes:in:)

Renders the glyphs at the specified positions, using the specified attributes.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedtvOS 9.0–13.0Deprecated

``` source
func showCGGlyphs(
    _ glyphs: UnsafePointer,
    positions: UnsafePointer,
    count glyphCount: Int,
    font: UIFont,
    matrix textMatrix: CGAffineTransform,
    attributes: [NSAttributedString.Key : Any] = [:],
    in graphicsContext: CGContext
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

