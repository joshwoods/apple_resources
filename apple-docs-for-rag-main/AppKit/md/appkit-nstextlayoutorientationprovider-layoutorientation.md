

- AppKit
- NSTextLayoutOrientationProvider
-  layoutOrientation 

Instance Property

# layoutOrientation

The default layout orientation.

macOS 10.7+

``` source
var layoutOrientation: NSLayoutManager.TextLayoutOrientation { get }
```

**Required**

## Discussion

This property contains the default layout orientation for text in the object that adopts the protocol. If the text contains an explicit verticalGlyphForm attribute, that attribute overrides the value in this property. When rendering, TextKit assumes the coordinate system is appropriately rotated.

## See Also

### Getting layout orientation

enum TextLayoutOrientation

Constants that describe the text layout orientation.

