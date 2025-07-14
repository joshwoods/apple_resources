

- UIKit
- UINavigationController
-  viewControllers 

Instance Property

# viewControllers

The view controllers currently on the navigation stack.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var viewControllers: [UIViewController] { get set }
```

## Discussion

The root view controller is at index `0` in the array, the back view controller is at index `n-2`, and the top controller is at index `n-1`, where `n` is the number of items in the array.

Assigning a new array of view controllers to this property is equivalent to calling the setViewControllers(_:animated:) method with the `animated` parameter set to false.

## See Also

### Accessing items on the navigation stack

var topViewController: UIViewController?

The view controller at the top of the navigation stack.

var visibleViewController: UIViewController?

The view controller associated with the currently visible view in the navigation interface.

func setViewControllers([UIViewController], animated: Bool)

Replaces the view controllers currently managed by the navigation controller with the specified items.

