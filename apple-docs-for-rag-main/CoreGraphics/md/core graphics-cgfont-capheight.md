

- Core Graphics
- CGFont
-  capHeight 

Instance Property

# capHeight

Returns the cap height of a font.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var capHeight: Int32 { get }
```

## Discussion

The cap height is the distance above the baseline of the top of flat capital letters of glyphs in a font. The value is specified in glyph space units.

## See Also

### Examining Font Metrics

var ascent: Int32

Returns the ascent of a font.

var descent: Int32

Returns the descent of a font.

var fontBBox: CGRect

Returns the bounding box of a font.

var italicAngle: CGFloat

Returns the italic angle of a font.

var leading: Int32

Returns the leading of a font.

var stemV: CGFloat

Returns the thickness of the dominant vertical stems of glyphs in a font.

var unitsPerEm: Int32

Returns the number of glyph space units per em for the provided font.

var xHeight: Int32

Returns the x-height of a font.

