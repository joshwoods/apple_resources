

- AppKit
- NSFont
-  descender 

Instance Property

# descender

The bottom y-coordinate, offset from the baseline, of the font’s longest descender.

macOS

``` source
var descender: CGFloat { get }
```

## Discussion

For example, if the longest descender extends 2 points below the baseline, the value in this property is `–2`.

## See Also

### Getting the Font Metrics

var ascender: CGFloat

The top y-coordinate, offset from the baseline, of the font’s longest ascender.

var capHeight: CGFloat

The cap height of the font.

var leading: CGFloat

The leading value of the font.

var xHeight: CGFloat

The x-height of the font.

