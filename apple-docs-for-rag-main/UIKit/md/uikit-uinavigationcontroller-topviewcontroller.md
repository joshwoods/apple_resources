

- UIKit
- UINavigationController
-  topViewController 

Instance Property

# topViewController

The view controller at the top of the navigation stack.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var topViewController: UIViewController? { get }
```

## See Also

### Accessing items on the navigation stack

var visibleViewController: UIViewController?

The view controller associated with the currently visible view in the navigation interface.

var viewControllers: [UIViewController]

The view controllers currently on the navigation stack.

func setViewControllers([UIViewController], animated: Bool)

Replaces the view controllers currently managed by the navigation controller with the specified items.

