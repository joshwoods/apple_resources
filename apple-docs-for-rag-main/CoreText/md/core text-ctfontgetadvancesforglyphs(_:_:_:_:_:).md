

- Core Text
-  CTFontGetAdvancesForGlyphs(\_:\_:\_:\_:\_:) 

Function

# CTFontGetAdvancesForGlyphs(\_:\_:\_:\_:\_:)

Calculates the advances for an array of glyphs and returns the summed advance.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontGetAdvancesForGlyphs(
    _ font: CTFont,
    _ orientation: CTFontOrientation,
    _ glyphs: UnsafePointer,
    _ advances: UnsafeMutablePointer?,
    _ count: CFIndex
) -> Double
```

## Parameters 

`font`  

The font reference.

`orientation`  

The intended drawing orientation of the glyphs. Used to determined which glyph metrics to return.

`glyphs`  

An array of `count` number of glyphs.

`advances`  

An array of `count` number of CGSize objects to receive the computed glyph advances. If `NULL`, only the overall advance is calculated.

`count`  

The capacity of the `glyphs` and `advances` buffers.

## Return Value

The summed glyph advance of an array of glyphs.

## Discussion

Individual glyph advances are passed back via the `advances` parameter. These are the ideal metrics for each glyph scaled and transformed in font space.

## See Also

### Getting Glyph Data

func CTFontCreatePathForGlyph(CTFont, CGGlyph, UnsafePointer&lt;CGAffineTransform>?) -> CGPath?

Creates a path for the specified glyph.

func CTFontGetGlyphWithName(CTFont, CFString) -> CGGlyph

Returns the glyph for the specified name.

func CTFontGetBoundingRectsForGlyphs(CTFont, CTFontOrientation, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGRect>?, CFIndex) -> CGRect

Calculates the bounding rects for an array of glyphs and returns the overall bounding rectangle for the glyph run.

func CTFontGetOpticalBoundsForGlyphs(CTFont, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGRect>?, CFIndex, CFOptionFlags) -> CGRect

Calculates the optical bounds for an array of glyphs and returns the overall optical bounds for the run.

func CTFontGetVerticalTranslationsForGlyphs(CTFont, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGSize>, CFIndex)

Calculates the offset from the default (horizontal) origin to the vertical origin for an array of glyphs.

