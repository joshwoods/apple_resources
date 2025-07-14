

- Core Text
-  CTFontGetVerticalTranslationsForGlyphs(\_:\_:\_:\_:) 

Function

# CTFontGetVerticalTranslationsForGlyphs(\_:\_:\_:\_:)

Calculates the offset from the default (horizontal) origin to the vertical origin for an array of glyphs.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontGetVerticalTranslationsForGlyphs(
    _ font: CTFont,
    _ glyphs: UnsafePointer,
    _ translations: UnsafeMutablePointer,
    _ count: CFIndex
)
```

## Parameters 

`font`  

The font reference.

`glyphs`  

An array of `count` number of glyphs.

`translations`  

On output, the computed origin offsets in an array of `count` number of CGSize objects.

`count`  

The capacity of the `glyphs` and `translations` buffers.

## See Also

### Getting Glyph Data

func CTFontCreatePathForGlyph(CTFont, CGGlyph, UnsafePointer&lt;CGAffineTransform>?) -> CGPath?

Creates a path for the specified glyph.

func CTFontGetGlyphWithName(CTFont, CFString) -> CGGlyph

Returns the glyph for the specified name.

func CTFontGetBoundingRectsForGlyphs(CTFont, CTFontOrientation, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGRect>?, CFIndex) -> CGRect

Calculates the bounding rects for an array of glyphs and returns the overall bounding rectangle for the glyph run.

func CTFontGetAdvancesForGlyphs(CTFont, CTFontOrientation, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGSize>?, CFIndex) -> Double

Calculates the advances for an array of glyphs and returns the summed advance.

func CTFontGetOpticalBoundsForGlyphs(CTFont, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGRect>?, CFIndex, CFOptionFlags) -> CGRect

Calculates the optical bounds for an array of glyphs and returns the overall optical bounds for the run.

