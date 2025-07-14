

- UIKit
- UIViewController
-  setNeedsUpdateOfHomeIndicatorAutoHidden() 

Instance Method

# setNeedsUpdateOfHomeIndicatorAutoHidden()

Notifies UIKit that your view controller updated its preference regarding the visual indicator for returning to the Home screen.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setNeedsUpdateOfHomeIndicatorAutoHidden()
```

## Discussion

When you change the value returned by your view controller’s prefersHomeIndicatorAutoHidden or childForHomeIndicatorAutoHidden method, call this method to let UIKit know that it should call those methods again.

## See Also

### Coordinating with system gestures

var preferredScreenEdgesDeferringSystemGestures: UIRectEdge

The screen edges for which you want your gestures to take precedence over the system gestures.

var childForScreenEdgesDeferringSystemGestures: UIViewController?

Returns the child view controller that should be queried to see if its gestures should take precedence.

func setNeedsUpdateOfScreenEdgesDeferringSystemGestures()

Notifies the system of changes to the screen edges that defer system gestures.

var prefersHomeIndicatorAutoHidden: Bool

A Boolean that indicates whether the system is allowed to hide the visual indicator for returning to the Home Screen.

var childForHomeIndicatorAutoHidden: UIViewController?

Returns the child view controller that is consulted about its preference for displaying a visual indicator for returning to the Home screen.

