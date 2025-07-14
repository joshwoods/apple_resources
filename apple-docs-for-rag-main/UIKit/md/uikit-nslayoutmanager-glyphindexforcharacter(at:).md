

- UIKit
- NSLayoutManager
-  glyphIndexForCharacter(at:) 

Instance Method

# glyphIndexForCharacter(at:)

Returns the index of the first glyph of the character at the specified index.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func glyphIndexForCharacter(at charIndex: Int) -> Int
```

## Parameters 

`charIndex`  

The index of the character for which to return the associated glyph.

## Return Value

The index of the first glyph associated with the character at the specified index.

## Discussion

If noncontiguous layout is not enabled, this method causes generation of all glyphs up to and including those associated with the specified character. This method accepts an index beyond the last character, returning an index extrapolated from the last actual character index.

In many cases it’s better to use the range-mapping methods, characterRange(forGlyphRange:actualGlyphRange:) and glyphRange(forCharacterRange:actualCharacterRange:), which provide more comprehensive information.

## See Also

### Accessing glyphs

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;CGGlyph>?, properties: UnsafeMutablePointer&lt;NSLayoutManager.GlyphProperty>?, characterIndexes: UnsafeMutablePointer&lt;Int>?, bidiLevels: UnsafeMutablePointer&lt;UInt8>?) -> Int

Fills a passed-in buffer with a sequence of glyphs.

func cgGlyph(at: Int) -> CGGlyph

Returns the glyph at the specified index.

func cgGlyph(at: Int, isValidIndex: UnsafeMutablePointer&lt;ObjCBool>?) -> CGGlyph

Returns the glyph at the specified index along with information about whether the glyph index is valid.

func setGlyphs(UnsafePointer&lt;CGGlyph>, properties: UnsafePointer&lt;NSLayoutManager.GlyphProperty>, characterIndexes: UnsafePointer&lt;Int>, font: UIFont, forGlyphRange: NSRange)

Stores the initial glyphs and glyph properties for a character range.

func characterIndexForGlyph(at: Int) -> Int

Returns the index in the text storage for the first character of the specified glyph.

func isValidGlyphIndex(Int) -> Bool

Indicates whether the specified index refers to a valid glyph.

var numberOfGlyphs: Int

The number of glyphs in the layout manager.

func propertyForGlyph(at: Int) -> NSLayoutManager.GlyphProperty

Returns the glyph property of the glyph at the specified index.

struct GlyphProperty

Glyph properties.

