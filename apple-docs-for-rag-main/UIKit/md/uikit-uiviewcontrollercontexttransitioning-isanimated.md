

- UIKit
- UIViewControllerContextTransitioning
-  isAnimated 

Instance Property

# isAnimated

A Boolean value indicating whether the transition should be animated.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var isAnimated: Bool { get }
```

**Required**

## Discussion

The value of this property is always true for modal presentation styles other than the UIModalPresentationStyle.custom style. When the modal presentation style is UIModalPresentationStyle.custom, the value is true if the transition should be animated or false if it should not. Use this value to determine whether you need to animate a custom transition into place, or whether you should install the final views into the container without animating the changes.

## See Also

### Getting the transition behaviors

var isInteractive: Bool

A Boolean value indicating whether the transition is currently interactive.

**Required**

var presentationStyle: UIModalPresentationStyle

Returns the presentation style for the view controller transition.

**Required**

