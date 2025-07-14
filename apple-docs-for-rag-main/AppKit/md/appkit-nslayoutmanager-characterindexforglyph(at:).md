

- AppKit
- NSLayoutManager
-  characterIndexForGlyph(at:) 

Instance Method

# characterIndexForGlyph(at:)

Returns the index in the text storage for the first character of the specified glyph.

macOS 10.7+

``` source
func characterIndexForGlyph(at glyphIndex: Int) -> Int
```

## Parameters 

`glyphIndex`  

The index of the glyph for which to return the associated character.

## Return Value

The index of the first character associated with the glyph at the specified index.

## Discussion

If noncontiguous layout is not enabled, this method causes generation of all glyphs up to and including `glyphIndex`. This method accepts an index beyond the last glyph, returning an index extrapolated from the last actual glyph index.

In many cases it’s better to use the range-mapping methods, characterRange(forGlyphRange:actualGlyphRange:) and glyphRange(forCharacterRange:actualCharacterRange:), which provide more comprehensive information.

## See Also

### Accessing glyphs

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;CGGlyph>?, properties: UnsafeMutablePointer&lt;NSLayoutManager.GlyphProperty>?, characterIndexes: UnsafeMutablePointer&lt;Int>?, bidiLevels: UnsafeMutablePointer&lt;UInt8>?) -> Int

Fills a passed-in buffer with a sequence of glyphs.

func cgGlyph(at: Int) -> CGGlyph

Returns the glyph at the specified index.

func cgGlyph(at: Int, isValidIndex: UnsafeMutablePointer&lt;ObjCBool>?) -> CGGlyph

Returns the glyph at the specified index along with information about whether the glyph index is valid.

func setGlyphs(UnsafePointer&lt;CGGlyph>, properties: UnsafePointer&lt;NSLayoutManager.GlyphProperty>, characterIndexes: UnsafePointer&lt;Int>, font: NSFont, forGlyphRange: NSRange)

Stores the initial glyphs and glyph properties for a character range.

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

