

- UIKit
- NSLayoutManager
-  getGlyphs(in:glyphs:properties:characterIndexes:bidiLevels:) 

Instance Method

# getGlyphs(in:glyphs:properties:characterIndexes:bidiLevels:)

Fills a passed-in buffer with a sequence of glyphs.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func getGlyphs(
    in glyphRange: NSRange,
    glyphs glyphBuffer: UnsafeMutablePointer?,
    properties props: UnsafeMutablePointer?,
    characterIndexes charIndexBuffer: UnsafeMutablePointer?,
    bidiLevels bidiLevelBuffer: UnsafeMutablePointer?
) -> Int
```

## Parameters 

`glyphRange`  

The range of glyphs to fill in.

`glyphBuffer`  

On output, the sequence of glyphs in the given glyph range.

`props`  

If not `NULL`, on output, the glyph properties corresponding to the filled-in glyphs.

`charIndexBuffer`  

If not `NULL`, on output, the indexes of the original characters corresponding to the given glyph range. Note that a glyph at index 1 is not necessarily mapped to the character at index 1, since a glyph may be for a ligature or accent.

`bidiLevelBuffer`  

If not `NULL`, on output, the direction of each glyph for bidirectional text. The values range from 0 to 61 as defined by Unicode Standard Annex \#9. An even value means the glyph goes left-to-right, and an odd value means the glyph goes right-to-left.

## Return Value

The number of glyphs returned in `glyphBuffer`.

## Discussion

Each pointer passed in should either be `NULL` or else point to sufficient memory to hold `glyphRange.length` elements.

## See Also

### Accessing glyphs

func cgGlyph(at: Int) -> CGGlyph

Returns the glyph at the specified index.

func cgGlyph(at: Int, isValidIndex: UnsafeMutablePointer&lt;ObjCBool>?) -> CGGlyph

Returns the glyph at the specified index along with information about whether the glyph index is valid.

func setGlyphs(UnsafePointer&lt;CGGlyph>, properties: UnsafePointer&lt;NSLayoutManager.GlyphProperty>, characterIndexes: UnsafePointer&lt;Int>, font: UIFont, forGlyphRange: NSRange)

Stores the initial glyphs and glyph properties for a character range.

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

