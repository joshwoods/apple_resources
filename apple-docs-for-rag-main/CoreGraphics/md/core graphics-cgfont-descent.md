

- Core Graphics
- CGFont
-  descent 

Instance Property

# descent

Returns the descent of a font.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var descent: Int32 { get }
```

## Discussion

The descent is the maximum distance below the baseline of glyphs in a font. The value is specified in glyph space units.

## See Also

### Examining Font Metrics

var ascent: Int32

Returns the ascent of a font.

var capHeight: Int32

Returns the cap height of a font.

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

