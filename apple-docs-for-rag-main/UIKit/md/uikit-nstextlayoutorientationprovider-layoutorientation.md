

- UIKit
- NSTextLayoutOrientationProvider
-  layoutOrientation 

Instance Property

# layoutOrientation

The default layout orientation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var layoutOrientation: NSLayoutManager.TextLayoutOrientation { get }
```

**Required**

## Discussion

This property contains the default layout orientation for text in the object that adopts the protocol. If the text contains an explicit verticalGlyphForm attribute in Swift or an NSVerticalGlyphFormAttributeName attribute in Objective-C, that attribute overrides the value in this property. When rendering, TextKit assumes the coordinate system is appropriately rotated.

## See Also

### Getting layout orientation

enum TextLayoutOrientation

Constants that describe the text layout orientation.

