

- AppKit
- NSFont
-  italicAngle 

Instance Property

# italicAngle

The number of degrees that the font is slanted counterclockwise from the vertical.

macOS

``` source
var italicAngle: CGFloat { get }
```

## Discussion

The italic angle value is read from the font’s AFM file. Because the slant is measured counterclockwise, English italic fonts typically return a negative value.

## See Also

### Getting Underline and Italic Metrics

var underlinePosition: CGFloat

The baseline offset to use when drawing underlines with the font.

var underlineThickness: CGFloat

The thickness to use when drawing underlines with the font.

