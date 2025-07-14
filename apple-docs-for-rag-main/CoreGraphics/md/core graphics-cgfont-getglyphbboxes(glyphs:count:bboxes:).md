

- Core Graphics
- CGFont
-  getGlyphBBoxes(glyphs:count:bboxes:) 

Instance Method

# getGlyphBBoxes(glyphs:count:bboxes:)

Get the bounding box of each glyph in an array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func getGlyphBBoxes(
    glyphs: UnsafePointer,
    count: Int,
    bboxes: UnsafeMutablePointer
) -> Bool
```

## Parameters 

`glyphs`  

A array of glyphs.

`count`  

The number of items in the `glyphs` array.

`bboxes`  

On return, the bounding boxes for each glyph.

## Return Value

`false` if bounding boxes can’t be retrieved for any reason; `true` otherwise.

## See Also

### Working with Glyphs

var numberOfGlyphs: Int

Returns the number of glyphs in a font.

func name(for: CGGlyph) -> CFString?

Returns the glyph name of the specified glyph in the specified font.

func getGlyphWithGlyphName(name: CFString) -> CGGlyph

Returns the glyph for the glyph name associated with the specified font object.

func getGlyphAdvances(glyphs: UnsafePointer&lt;CGGlyph>, count: Int, advances: UnsafeMutablePointer&lt;Int32>) -> Bool

Gets the advance width of each glyph in the provided array.

typealias CGGlyph

An index into the internal glyph table of a font.

let kCGGlyphMax: CGFontIndex

The maximum allowed value of a CGGlyph.

typealias CGFontIndex

An index into a font table.

let kCGFontIndexMax: CGFontIndex

The maximum allowed value of a CGFontIndex.

let kCGFontIndexInvalid: CGFontIndex

An invalid font index (a value which never represents a valid glyph).

