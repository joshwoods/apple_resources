

- UIKit
- UIView
-  largeContentTitle 

Instance Property

# largeContentTitle

A string that describes the view in the large content viewer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var largeContentTitle: String? { get set }
```

## Discussion

To present content in the large content viewer, you can provide either largeContentTitle or largeContentImage, or both.

This property defaults to an appropriate value for UIKit classes; otherwise, it’s `nil`.

## See Also

### Modifying the accessibility behavior

var accessibilityIgnoresInvertColors: Bool

A Boolean value indicating whether the view ignores an accessibility request to invert its colors.

var largeContentImage: UIImage?

An image that represents the view in the large content viewer.

var largeContentImageInsets: UIEdgeInsets

Insets to adjust the position of the view’s image so it appears centered in the large content viewer.

var scalesLargeContentImage: Bool

A Boolean value that indicates whether the large content viewer scales the item’s image to a larger size.

var showsLargeContentViewer: Bool

A Boolean value that indicates whether to show the view in the large content viewer.

