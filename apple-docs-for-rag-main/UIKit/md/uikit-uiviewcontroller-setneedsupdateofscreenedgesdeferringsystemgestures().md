

- UIKit
- UIViewController
-  setNeedsUpdateOfScreenEdgesDeferringSystemGestures() 

Instance Method

# setNeedsUpdateOfScreenEdgesDeferringSystemGestures()

Notifies the system of changes to the screen edges that defer system gestures.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setNeedsUpdateOfScreenEdgesDeferringSystemGestures()
```

## Discussion

Call this method whenever you modify the screen edges that defer system gestures, such as those that invoke Control Center, so the system can update accordingly. If the childForScreenEdgesDeferringSystemGestures property is `nil`, the system reads the edges from the current view controller’s preferredScreenEdgesDeferringSystemGestures property; otherwise, it uses the same property on the referenced child view controller.

## See Also

### Coordinating with system gestures

var preferredScreenEdgesDeferringSystemGestures: UIRectEdge

The screen edges for which you want your gestures to take precedence over the system gestures.

var childForScreenEdgesDeferringSystemGestures: UIViewController?

Returns the child view controller that should be queried to see if its gestures should take precedence.

var prefersHomeIndicatorAutoHidden: Bool

A Boolean that indicates whether the system is allowed to hide the visual indicator for returning to the Home Screen.

var childForHomeIndicatorAutoHidden: UIViewController?

Returns the child view controller that is consulted about its preference for displaying a visual indicator for returning to the Home screen.

func setNeedsUpdateOfHomeIndicatorAutoHidden()

Notifies UIKit that your view controller updated its preference regarding the visual indicator for returning to the Home screen.

