

- UIKit
- UIPageViewController
-  gestureRecognizers 

Instance Property

# gestureRecognizers

An array of UIGestureRecognizer objects that are configured to handle user interaction.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var gestureRecognizers: [UIGestureRecognizer] { get }
```

## Discussion

These gesture recognizers are initially attached to a view in the page view controller’s hierarchy. To change the region of the screen in which the user can navigate using gestures, they can be placed on another view.

## See Also

### Providing Content

func setViewControllers([UIViewController]?, direction: UIPageViewController.NavigationDirection, animated: Bool, completion: ((Bool) -> Void)?)

Sets the view controllers to be displayed.

enum NavigationDirection

Directions for page-turn transitions.

var viewControllers: [UIViewController]?

The view controllers displayed by the page view controller.

