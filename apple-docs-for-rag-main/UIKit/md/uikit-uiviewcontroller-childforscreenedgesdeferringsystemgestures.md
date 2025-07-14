

- UIKit
- UIViewController
-  childForScreenEdgesDeferringSystemGestures 

Instance Property

# childForScreenEdgesDeferringSystemGestures

Returns the child view controller that should be queried to see if its gestures should take precedence.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var childForScreenEdgesDeferringSystemGestures: UIViewController? { get }
```

## Mentioned in 

Creating a custom container view controller

## Discussion

When implementing a container view controller, override this method if one of your child view controllers defines screen-edge gestures that should take precedence over the system gestures. UIKit then uses the preferredScreenEdgesDeferringSystemGestures property of the returned child view controller to determine which screen edges have competing gesture recognizers.

## See Also

### Coordinating with system gestures

var preferredScreenEdgesDeferringSystemGestures: UIRectEdge

The screen edges for which you want your gestures to take precedence over the system gestures.

func setNeedsUpdateOfScreenEdgesDeferringSystemGestures()

Notifies the system of changes to the screen edges that defer system gestures.

var prefersHomeIndicatorAutoHidden: Bool

A Boolean that indicates whether the system is allowed to hide the visual indicator for returning to the Home Screen.

var childForHomeIndicatorAutoHidden: UIViewController?

Returns the child view controller that is consulted about its preference for displaying a visual indicator for returning to the Home screen.

func setNeedsUpdateOfHomeIndicatorAutoHidden()

Notifies UIKit that your view controller updated its preference regarding the visual indicator for returning to the Home screen.

