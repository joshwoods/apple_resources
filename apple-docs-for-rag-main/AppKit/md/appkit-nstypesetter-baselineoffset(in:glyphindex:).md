

- AppKit
- NSTypesetter
-  baselineOffset(in:glyphIndex:) 

Instance Method

# baselineOffset(in:glyphIndex:)

Returns the distance from the bottom of the line fragment rectangle in which the glyph resides to the glyph baseline.

macOS

``` source
func baselineOffset(
    in layoutMgr: NSLayoutManager,
    glyphIndex: Int
) -> CGFloat
```

## Parameters 

`layoutMgr`  

The layout manager used for the drawing.

`glyphIndex`  

The index of the glyph in question.

## Return Value

The distance from the bottom of the line fragment rectangle in which the glyph resides to the glyph baseline.

## Discussion

The text system uses this value to calculate the vertical position of underlines.

## See Also

### Getting information about glyphs

class func printingAdjustment(in: NSLayoutManager, forNominallySpacedGlyphRange: NSRange, packedGlyphs: UnsafePointer&lt;UInt8>, count: Int) -> NSSize

Returns the interglyph spacing in the specified range when sent to a printer.

