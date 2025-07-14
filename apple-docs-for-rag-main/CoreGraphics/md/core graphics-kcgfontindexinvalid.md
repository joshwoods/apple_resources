

- Core Graphics
-  kCGFontIndexInvalid 

Global Variable

# kCGFontIndexInvalid

An invalid font index (a value which never represents a valid glyph).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCGFontIndexInvalid: CGFontIndex
```

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

