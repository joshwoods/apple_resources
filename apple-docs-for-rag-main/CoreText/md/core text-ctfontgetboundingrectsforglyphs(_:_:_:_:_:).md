

- Core Text
-  CTFontGetBoundingRectsForGlyphs(\_:\_:\_:\_:\_:) 

Function

# CTFontGetBoundingRectsForGlyphs(\_:\_:\_:\_:\_:)

Calculates the bounding rects for an array of glyphs and returns the overall bounding rectangle for the glyph run.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontGetBoundingRectsForGlyphs(
    _ font: CTFont,
    _ orientation: CTFontOrientation,
    _ glyphs: UnsafePointer,
    _ boundingRects: UnsafeMutablePointer?,
    _ count: CFIndex
) -> CGRect
```

## Parameters 

`font`  

The font reference.

`orientation`  

The intended drawing orientation of the glyphs. Used to determined which glyph metrics to return.

`glyphs`  

An array of `count` number of glyphs.

`boundingRects`  

On output, the computed glyph rectangles in an array of `count` number of CGRect objects. If `NULL`, only the overall bounding rectangle is calculated.

`count`  

The capacity of the `glyphs` and `boundingRects` buffers.

## Return Value

The overall bounding rectangle for an array or run of glyphs. Returns CGRectNull on error.

## Discussion

The bounding rectangles of the individual glyphs are returned through the `boundingRects` parameter. These are the design metrics from the font transformed in font space.

## See Also

### Getting Glyph Data

func CTFontCreatePathForGlyph(CTFont, CGGlyph, UnsafePointer&lt;CGAffineTransform>?) -> CGPath?

Creates a path for the specified glyph.

func CTFontGetGlyphWithName(CTFont, CFString) -> CGGlyph

Returns the glyph for the specified name.

func CTFontGetAdvancesForGlyphs(CTFont, CTFontOrientation, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGSize>?, CFIndex) -> Double

Calculates the advances for an array of glyphs and returns the summed advance.

func CTFontGetOpticalBoundsForGlyphs(CTFont, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGRect>?, CFIndex, CFOptionFlags) -> CGRect

Calculates the optical bounds for an array of glyphs and returns the overall optical bounds for the run.

func CTFontGetVerticalTranslationsForGlyphs(CTFont, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGSize>, CFIndex)

Calculates the offset from the default (horizontal) origin to the vertical origin for an array of glyphs.

