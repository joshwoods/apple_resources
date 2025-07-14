

- AppKit
- NSFont
-  underlinePosition 

Instance Property

# underlinePosition

The baseline offset to use when drawing underlines with the font.

macOS

``` source
var underlinePosition: CGFloat { get }
```

## Discussion

The value in this property is determined by the font’s AFM file. The value is usually negative, which must be considered when drawing in a flipped coordinate system.

## See Also

### Getting Underline and Italic Metrics

var italicAngle: CGFloat

The number of degrees that the font is slanted counterclockwise from the vertical.

var underlineThickness: CGFloat

The thickness to use when drawing underlines with the font.

