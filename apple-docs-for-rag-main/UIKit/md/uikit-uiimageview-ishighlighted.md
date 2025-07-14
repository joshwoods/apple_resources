

- UIKit
- UIImageView
-  isHighlighted 

Instance Property

# isHighlighted

A Boolean value that determines whether the image is highlighted.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isHighlighted: Bool { get set }
```

## Discussion

This property determines whether the regular or highlighted images are used. When isHighlighted is set to true, a non-animated image will use the highlightedImage property and an animated image will use the highlightedAnimationImages. If both of those properties are set to `nil` or if isHighlighted is set to false, it will use the image and animationImages properties.

## See Also

### Configuring the image view

var isUserInteractionEnabled: Bool

A Boolean value that determines whether user events are ignored and removed from the event queue.

var tintColor: UIColor!

A color used to tint template images in the view hierarchy.

