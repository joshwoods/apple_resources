

- AppKit
- NSLayoutManager
-  isValidGlyphIndex(\_:) 

Instance Method

# isValidGlyphIndex(\_:)

Indicates whether the specified index refers to a valid glyph.

macOS 10.0+

``` source
func isValidGlyphIndex(_ glyphIndex: Int) -> Bool
```

## Parameters 

`glyphIndex`  

The index of a glyph in the receiver.

## Return Value

true if the specified `glyphIndex` refers to a valid glyph, otherwise false.

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

var numberOfGlyphs: Int

The number of glyphs in the layout manager.

func propertyForGlyph(at: Int) -> NSLayoutManager.GlyphProperty

Returns the glyph property of the glyph at the specified index.

struct GlyphProperty

Glyph properties.

