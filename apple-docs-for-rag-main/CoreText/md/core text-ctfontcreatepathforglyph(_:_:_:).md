

- Core Text
-  CTFontCreatePathForGlyph(\_:\_:\_:) 

Function

# CTFontCreatePathForGlyph(\_:\_:\_:)

Creates a path for the specified glyph.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCreatePathForGlyph(
    _ font: CTFont,
    _ glyph: CGGlyph,
    _ matrix: UnsafePointer?
) -> CGPath?
```

## Parameters 

`font`  

The font reference.

`glyph`  

The glyph.

`matrix`  

An affine transform applied to the path. Can be `NULL`. If `NULL`, CGAffineTransformIdentity is used.

## Return Value

A CGPath object containing the glyph outlines, `NULL` on error. Must be released by caller.

## Discussion

Creates a path from the outlines of the glyph for the specified font. The path reflects the font point size, matrix, and transform parameter, applied in that order. The transform parameter is most commonly be used to provide a translation to the desired glyph origin.

## See Also

### Getting Glyph Data

func CTFontGetGlyphWithName(CTFont, CFString) -> CGGlyph

Returns the glyph for the specified name.

func CTFontGetBoundingRectsForGlyphs(CTFont, CTFontOrientation, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGRect>?, CFIndex) -> CGRect

Calculates the bounding rects for an array of glyphs and returns the overall bounding rectangle for the glyph run.

func CTFontGetAdvancesForGlyphs(CTFont, CTFontOrientation, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGSize>?, CFIndex) -> Double

Calculates the advances for an array of glyphs and returns the summed advance.

func CTFontGetOpticalBoundsForGlyphs(CTFont, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGRect>?, CFIndex, CFOptionFlags) -> CGRect

Calculates the optical bounds for an array of glyphs and returns the overall optical bounds for the run.

func CTFontGetVerticalTranslationsForGlyphs(CTFont, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGSize>, CFIndex)

Calculates the offset from the default (horizontal) origin to the vertical origin for an array of glyphs.

