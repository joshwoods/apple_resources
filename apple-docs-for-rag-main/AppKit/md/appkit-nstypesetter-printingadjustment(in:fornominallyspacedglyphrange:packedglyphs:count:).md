

- AppKit
- NSTypesetter
-  printingAdjustment(in:forNominallySpacedGlyphRange:packedGlyphs:count:) 

Type Method

# printingAdjustment(in:forNominallySpacedGlyphRange:packedGlyphs:count:)

Returns the interglyph spacing in the specified range when sent to a printer.

macOS

``` source
class func printingAdjustment(
    in layoutMgr: NSLayoutManager,
    forNominallySpacedGlyphRange nominallySpacedGlyphsRange: NSRange,
    packedGlyphs: UnsafePointer,
    count packedGlyphsCount: Int
) -> NSSize
```

## Parameters 

`layoutMgr`  

The layout manager that will do the drawing.

`nominallySpacedGlyphsRange`  

The range of the glyphs whose spacing is desired.

`packedGlyphs`  

The glyphs as they are packed for sending to be drawn in `layoutMgr`.

`packedGlyphsCount`  

The number of glyphs in `packedGlyphs`.

## Return Value

The interglyph spacing in the specified range when sent to a printer. If the font metrics of the font used for displaying text on the screen is different from the font metrics of the font used in printing, then this interglyph spacing may need to be adjusted slightly to match that used on the screen.

## See Also

### Getting information about glyphs

func baselineOffset(in: NSLayoutManager, glyphIndex: Int) -> CGFloat

Returns the distance from the bottom of the line fragment rectangle in which the glyph resides to the glyph baseline.

