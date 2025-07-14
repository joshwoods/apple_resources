

- UIKit
- UIView
-  showsLargeContentViewer 

Instance Property

# showsLargeContentViewer

A Boolean value that indicates whether to show the view in the large content viewer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var showsLargeContentViewer: Bool { get set }
```

## Discussion

For this property to take effect, the view must have a UILargeContentViewerInteraction.

## See Also

### Modifying the accessibility behavior

var accessibilityIgnoresInvertColors: Bool

A Boolean value indicating whether the view ignores an accessibility request to invert its colors.

var largeContentImage: UIImage?

An image that represents the view in the large content viewer.

var largeContentImageInsets: UIEdgeInsets

Insets to adjust the position of the view’s image so it appears centered in the large content viewer.

var largeContentTitle: String?

A string that describes the view in the large content viewer.

var scalesLargeContentImage: Bool

A Boolean value that indicates whether the large content viewer scales the item’s image to a larger size.

