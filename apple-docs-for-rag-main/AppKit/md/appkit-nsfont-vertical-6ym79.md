

- AppKit
- NSFont
-  vertical 

Instance Property

# vertical

A vertical version of the font.

macOS 10.7+

``` source
@NSCopying
var vertical: NSFont { get }
```

## Discussion

The value in this property is a vertical version of the font, if such a configuration is supported. If a vertical configuration is not supported, the value in the property is `self`.

A vertical font applies appropriate rotation to the text matrix in set(in:), returns vertical metrics, and enables the vertical glyph substitution feature by default.

## See Also

### Vertical Fonts

var isVertical: Bool

A Boolean value indicating whether the font is a vertical font.

