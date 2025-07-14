

- UIKit
- UIPageViewController
-  viewControllers 

Instance Property

# viewControllers

The view controllers displayed by the page view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var viewControllers: [UIViewController]? { get }
```

## See Also

### Providing Content

func setViewControllers([UIViewController]?, direction: UIPageViewController.NavigationDirection, animated: Bool, completion: ((Bool) -> Void)?)

Sets the view controllers to be displayed.

enum NavigationDirection

Directions for page-turn transitions.

var gestureRecognizers: [UIGestureRecognizer]

An array of UIGestureRecognizer objects that are configured to handle user interaction.

