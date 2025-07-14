

- UIKit
- UIFont
-  descender 

Instance Property

# descender

The bottom y-coordinate, offset from the baseline, of the font’s longest descender.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var descender: CGFloat { get }
```

## Discussion

The descender value is measured in points. This value may be positive or negative. For example, if the longest descender extends 2 points below the baseline, this method returns `-2.0` .

## See Also

### Getting Font Metrics

var pointSize: CGFloat

The font’s point size, or the effective vertical point size for a font with a nonstandard matrix.

var ascender: CGFloat

The top y-coordinate, offset from the baseline, of the font’s longest ascender.

var leading: CGFloat

The font’s leading information.

var capHeight: CGFloat

The font’s cap height information.

var xHeight: CGFloat

The x-height of the font.

var lineHeight: CGFloat

The height, in points, of text lines.

