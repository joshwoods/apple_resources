

- AppKit
- NSLayoutManager
-  propertyForGlyph(at:) 

Instance Method

# propertyForGlyph(at:)

Returns the glyph property of the glyph at the specified index.

macOS 10.5+

``` source
func propertyForGlyph(at glyphIndex: Int) -> NSLayoutManager.GlyphProperty
```

## Parameters 

`glyphIndex`  

The glyph whose glyph property is returned.

## Return Value

The glyph property associated with the specified glyph. NSLayoutManager.GlyphProperty lists the values that can be returned.

## Discussion

If noncontiguous layout is not enabled, this method causes generation of all glyphs up to and including the one at `glyphIndex`.

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

func characterIndexForGlyph(at: Int) -> Int

Returns the index in the text storage for the first character of the specified glyph.

func glyphIndexForCharacter(at: Int) -> Int

Returns the index of the first glyph of the character at the specified index.

func isValidGlyphIndex(Int) -> Bool

Indicates whether the specified index refers to a valid glyph.

var numberOfGlyphs: Int

The number of glyphs in the layout manager.

struct GlyphProperty

Glyph properties.

