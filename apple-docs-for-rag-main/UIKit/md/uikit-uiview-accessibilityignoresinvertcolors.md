

- UIKit
- UIView
-  accessibilityIgnoresInvertColors 

Instance Property

# accessibilityIgnoresInvertColors

A Boolean value indicating whether the view ignores an accessibility request to invert its colors.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var accessibilityIgnoresInvertColors: Bool { get set }
```

## Discussion

Inverting colors is often used to help users with light or color sensitivities to make bright colors darker. However, this behavior can have a destructive impact on images and videos. If inverting the colors would have a negative impact on your view’s content, set this property to true to prevent it from inverting its colors. Setting the property to true prevents the system from inverting the colors of the view and all of its subviews.

## See Also

### Modifying the accessibility behavior

var largeContentImage: UIImage?

An image that represents the view in the large content viewer.

var largeContentImageInsets: UIEdgeInsets

Insets to adjust the position of the view’s image so it appears centered in the large content viewer.

var largeContentTitle: String?

A string that describes the view in the large content viewer.

var scalesLargeContentImage: Bool

A Boolean value that indicates whether the large content viewer scales the item’s image to a larger size.

var showsLargeContentViewer: Bool

A Boolean value that indicates whether to show the view in the large content viewer.

