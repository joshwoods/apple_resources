

- UIKit
- NSLayoutManager
-  setGlyphs(\_:properties:characterIndexes:font:forGlyphRange:) 

Instance Method

# setGlyphs(\_:properties:characterIndexes:font:forGlyphRange:)

Stores the initial glyphs and glyph properties for a character range.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func setGlyphs(
    _ glyphs: UnsafePointer,
    properties props: UnsafePointer,
    characterIndexes charIndexes: UnsafePointer,
    font aFont: UIFont,
    forGlyphRange glyphRange: NSRange
)
```

## Parameters 

`glyphs`  

A pointer to the layout manager’s glyph cache.

`props`  

A pointer to a buffer containing glyph properties for the glyphs in the cache.

`charIndexes`  

A pointer to the starting index for the characters in the text storage for which glyphs are generated.

`aFont`  

A font to override the font attributes in the text storage for the specified character range.

`glyphRange`  

The range of glyphs in the glyph cache to set.

## Discussion

This method is invoked by text system during the glyph generation process. The only place apps are allowed to call this method directly is from an implementation of the `NSLayoutManagerDelegate` protocol method layoutManager(_:shouldGenerateGlyphs:properties:characterIndexes:font:forGlyphRange:).

Each array has `glyphRange.length` items. The specified `charIndexes` must be contiguous (no skipped indexes), enabling multiple items to have a same character index (as when one character index generates multiple glyph IDs). Due to font substitution, `aFont` passed into this method might not match the font in the attributes dictionary. Calling this method for a character range that has previously calculated layout information invalidates the layout and display.

## See Also

### Accessing glyphs

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;CGGlyph>?, properties: UnsafeMutablePointer&lt;NSLayoutManager.GlyphProperty>?, characterIndexes: UnsafeMutablePointer&lt;Int>?, bidiLevels: UnsafeMutablePointer&lt;UInt8>?) -> Int

Fills a passed-in buffer with a sequence of glyphs.

func cgGlyph(at: Int) -> CGGlyph

Returns the glyph at the specified index.

func cgGlyph(at: Int, isValidIndex: UnsafeMutablePointer&lt;ObjCBool>?) -> CGGlyph

Returns the glyph at the specified index along with information about whether the glyph index is valid.

func characterIndexForGlyph(at: Int) -> Int

Returns the index in the text storage for the first character of the specified glyph.

func glyphIndexForCharacter(at: Int) -> Int

Returns the index of the first glyph of the character at the specified index.

func isValidGlyphIndex(Int) -> Bool

Indicates whether the specified index refers to a valid glyph.

var numberOfGlyphs: Int

The number of glyphs in the layout manager.

func propertyForGlyph(at: Int) -> NSLayoutManager.GlyphProperty

Returns the glyph property of the glyph at the specified index.

struct GlyphProperty

Glyph properties.

