

- UIKit
- UIImageView
-  isUserInteractionEnabled 

Instance Property

# isUserInteractionEnabled

A Boolean value that determines whether user events are ignored and removed from the event queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isUserInteractionEnabled: Bool { get set }
```

## Discussion

This property is inherited from the UIView parent class. This class changes the default value of this property to false.

## See Also

### Configuring the image view

var isHighlighted: Bool

A Boolean value that determines whether the image is highlighted.

var tintColor: UIColor!

A color used to tint template images in the view hierarchy.

