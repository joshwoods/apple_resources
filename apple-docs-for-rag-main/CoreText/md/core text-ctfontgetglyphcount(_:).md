

- Core Text
-  CTFontGetGlyphCount(\_:) 

Function

# CTFontGetGlyphCount(\_:)

Returns the number of glyphs of the given font.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontGetGlyphCount(_ font: CTFont) -> CFIndex
```

## Parameters 

`font`  

The font reference.

## Return Value

The number of glyphs in the font.

## See Also

### Getting Font Metrics

func CTFontGetAscent(CTFont) -> CGFloat

Returns the scaled font-ascent metric of the given font.

func CTFontGetDescent(CTFont) -> CGFloat

Returns the scaled font-descent metric of the given font.

func CTFontGetLeading(CTFont) -> CGFloat

Returns the scaled font-leading metric of the given font.

func CTFontGetUnitsPerEm(CTFont) -> UInt32

Returns the units-per-em metric of the given font.

func CTFontGetBoundingBox(CTFont) -> CGRect

Returns the scaled bounding box of the given font.

func CTFontGetUnderlinePosition(CTFont) -> CGFloat

Returns the scaled underline position of the given font.

func CTFontGetUnderlineThickness(CTFont) -> CGFloat

Returns the scaled underline-thickness metric of the given font.

func CTFontGetSlantAngle(CTFont) -> CGFloat

Returns the slant angle of the given font.

func CTFontGetCapHeight(CTFont) -> CGFloat

Returns the cap-height metric of the given font.

func CTFontGetXHeight(CTFont) -> CGFloat

Returns the x-height metric of the given font.

