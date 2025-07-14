

- UIKit
- UINavigationController
-  visibleViewController 

Instance Property

# visibleViewController

The view controller associated with the currently visible view in the navigation interface.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var visibleViewController: UIViewController? { get }
```

## Discussion

The currently visible view can belong either to the view controller at the top of the navigation stack or to a view controller that was presented modally on top of the navigation controller itself.

## See Also

### Accessing items on the navigation stack

var topViewController: UIViewController?

The view controller at the top of the navigation stack.

var viewControllers: [UIViewController]

The view controllers currently on the navigation stack.

func setViewControllers([UIViewController], animated: Bool)

Replaces the view controllers currently managed by the navigation controller with the specified items.

