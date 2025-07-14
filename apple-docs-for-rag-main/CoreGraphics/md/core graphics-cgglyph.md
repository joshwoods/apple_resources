

- Core Graphics
-  CGGlyph 

Type Alias

# CGGlyph

An index into the internal glyph table of a font.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGGlyph = CGFontIndex
```

## Discussion

When drawing text, you typically specify a sequence of characters. However, Core Graphics also allows you to use CGGlyph values to specify glyphs. In either case, Core Graphics renders the text using font data provided by the Apple Type Services (ATS) framework.

You provide CGGlyph values to the functions showGlyphs(g:count:) and showGlyphsAtPoint(x:y:glyphs:count:). These functions display an array of glyphs at the current text position or at a position you specify, respectively.

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

let kCGGlyphMax: CGFontIndex

The maximum allowed value of a CGGlyph.

typealias CGFontIndex

An index into a font table.

let kCGFontIndexMax: CGFontIndex

The maximum allowed value of a CGFontIndex.

let kCGFontIndexInvalid: CGFontIndex

An invalid font index (a value which never represents a valid glyph).

