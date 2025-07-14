

- UIKit
- UIViewControllerContextTransitioning
-  isInteractive 

Instance Property

# isInteractive

A Boolean value indicating whether the transition is currently interactive.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var isInteractive: Bool { get }
```

**Required**

## Discussion

A transition is interactive only if the view controller’s delegate provides a corresponding interactive animator object.

Interactive transitions are drive by user-generated events. One common scenario is to use a gesture recognizer to report on the current progress of the animation. The gesture recognizer calls methods of this context object that indicate the completion percentage of the transition or indicate that the transition was canceled or completed by the user.

## See Also

### Getting the transition behaviors

var isAnimated: Bool

A Boolean value indicating whether the transition should be animated.

**Required**

var presentationStyle: UIModalPresentationStyle

Returns the presentation style for the view controller transition.

**Required**

