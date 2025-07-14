

- UIKit
- UIImageView
-  tintColor 

Instance Property

# tintColor

A color used to tint template images in the view hierarchy.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var tintColor: UIColor! { get set }
```

## Discussion

The default is `nil`. If a non-`nil` value is specified, the color is applied to any template images attached to the image view. For more information, see the renderingMode property on the UIImage class.

## See Also

### Configuring the image view

var isUserInteractionEnabled: Bool

A Boolean value that determines whether user events are ignored and removed from the event queue.

var isHighlighted: Bool

A Boolean value that determines whether the image is highlighted.

