

- Core Graphics
- CGFont
-  getGlyphAdvances(glyphs:count:advances:) 

Instance Method

# getGlyphAdvances(glyphs:count:advances:)

Gets the advance width of each glyph in the provided array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func getGlyphAdvances(
    glyphs: UnsafePointer,
    count: Int,
    advances: UnsafeMutablePointer
) -> Bool
```

## Parameters 

`glyphs`  

An array of glyphs.

`count`  

The number of glyphs in the array.

`advances`  

On output, an array of advance widths for the provided glyphs.

## Return Value

true unless the advance widths can’t be provided for some reason.

## See Also

### Working with Glyphs

var numberOfGlyphs: Int

Returns the number of glyphs in a font.

func name(for: CGGlyph) -> CFString?

Returns the glyph name of the specified glyph in the specified font.

func getGlyphWithGlyphName(name: CFString) -> CGGlyph

Returns the glyph for the glyph name associated with the specified font object.

func getGlyphBBoxes(glyphs: UnsafePointer&lt;CGGlyph>, count: Int, bboxes: UnsafeMutablePointer&lt;CGRect>) -> Bool

Get the bounding box of each glyph in an array.

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

