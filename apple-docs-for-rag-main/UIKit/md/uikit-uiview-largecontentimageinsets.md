

- UIKit
- UIView
-  largeContentImageInsets 

Instance Property

# largeContentImageInsets

Insets to adjust the position of the view’s image so it appears centered in the large content viewer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var largeContentImageInsets: UIEdgeInsets { get set }
```

## Discussion

This property defaults to zero.

## See Also

### Modifying the accessibility behavior

var accessibilityIgnoresInvertColors: Bool

A Boolean value indicating whether the view ignores an accessibility request to invert its colors.

var largeContentImage: UIImage?

An image that represents the view in the large content viewer.

var largeContentTitle: String?

A string that describes the view in the large content viewer.

var scalesLargeContentImage: Bool

A Boolean value that indicates whether the large content viewer scales the item’s image to a larger size.

var showsLargeContentViewer: Bool

A Boolean value that indicates whether to show the view in the large content viewer.

