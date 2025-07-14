

- UIKit
- UIViewController
-  childForHomeIndicatorAutoHidden 

Instance Property

# childForHomeIndicatorAutoHidden

Returns the child view controller that is consulted about its preference for displaying a visual indicator for returning to the Home screen.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var childForHomeIndicatorAutoHidden: UIViewController? { get }
```

## Return Value

The child view controller to consult. The default implementation of this method returns `nil`.

## Mentioned in 

Creating a custom container view controller

## Discussion

When implementing a container view controller, override this method if you want one your child view controllers to determine whether to display the visual indicator. If you do, the system calls the prefersHomeIndicatorAutoHidden method of the returned view controller. If the method returns `nil`, the system calls the prefersHomeIndicatorAutoHidden method of the current view controller.

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

func setNeedsUpdateOfHomeIndicatorAutoHidden()

Notifies UIKit that your view controller updated its preference regarding the visual indicator for returning to the Home screen.

