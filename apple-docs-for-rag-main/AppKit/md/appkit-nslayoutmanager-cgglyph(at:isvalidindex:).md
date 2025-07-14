

- AppKit
- NSLayoutManager
-  cgGlyph(at:isValidIndex:) 

Instance Method

# cgGlyph(at:isValidIndex:)

Returns the glyph at the specified index along with information about whether the glyph index is valid.

macOS 10.11+

``` source
func cgGlyph(
    at glyphIndex: Int,
    isValidIndex: UnsafeMutablePointer?
) -> CGGlyph
```

## Parameters 

`glyphIndex`  

The index of the glyph that you want.

`isValidIndex`  

An optional Boolean variable. On return, the variable is set to true if the glyph index is valid or false if it is not.

## Return Value

The glyph at the specified index or kCGFontIndexInvalid if the index is out of range.

## Discussion

If noncontiguous layout is disabled, calling this method generates all glyphs up to and including the one at `glyphIndex`.

## See Also

### Accessing glyphs

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;CGGlyph>?, properties: UnsafeMutablePointer&lt;NSLayoutManager.GlyphProperty>?, characterIndexes: UnsafeMutablePointer&lt;Int>?, bidiLevels: UnsafeMutablePointer&lt;UInt8>?) -> Int

Fills a passed-in buffer with a sequence of glyphs.

func cgGlyph(at: Int) -> CGGlyph

Returns the glyph at the specified index.

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

func propertyForGlyph(at: Int) -> NSLayoutManager.GlyphProperty

Returns the glyph property of the glyph at the specified index.

struct GlyphProperty

Glyph properties.

