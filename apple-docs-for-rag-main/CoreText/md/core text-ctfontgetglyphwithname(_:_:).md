

- Core Text
-  CTFontGetGlyphWithName(\_:\_:) 

Function

# CTFontGetGlyphWithName(\_:\_:)

Returns the glyph for the specified name.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontGetGlyphWithName(
    _ font: CTFont,
    _ glyphName: CFString
) -> CGGlyph
```

## Parameters 

`font`  

The font reference.

`glyphName`  

The glyph name as a `CFString` object.

## Return Value

The glyph value for the named glyph as a CGGlyph object, or if the glyph name is not recognized, the `.notdef` glyph index value.

## Discussion

The returned `CGGlyph` object can be used with any of the subsequent glyph data accessors or directly with Core Graphics.

## See Also

### Getting Glyph Data

func CTFontCreatePathForGlyph(CTFont, CGGlyph, UnsafePointer&lt;CGAffineTransform>?) -> CGPath?

Creates a path for the specified glyph.

func CTFontGetBoundingRectsForGlyphs(CTFont, CTFontOrientation, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGRect>?, CFIndex) -> CGRect

Calculates the bounding rects for an array of glyphs and returns the overall bounding rectangle for the glyph run.

func CTFontGetAdvancesForGlyphs(CTFont, CTFontOrientation, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGSize>?, CFIndex) -> Double

Calculates the advances for an array of glyphs and returns the summed advance.

func CTFontGetOpticalBoundsForGlyphs(CTFont, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGRect>?, CFIndex, CFOptionFlags) -> CGRect

Calculates the optical bounds for an array of glyphs and returns the overall optical bounds for the run.

func CTFontGetVerticalTranslationsForGlyphs(CTFont, UnsafePointer&lt;CGGlyph>, UnsafeMutablePointer&lt;CGSize>, CFIndex)

Calculates the offset from the default (horizontal) origin to the vertical origin for an array of glyphs.

