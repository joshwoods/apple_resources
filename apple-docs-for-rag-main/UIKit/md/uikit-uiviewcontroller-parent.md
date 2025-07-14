

- UIKit
- UIViewController
-  parent 

Instance Property

# parent

The parent view controller of the recipient.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var parent: UIViewController? { get }
```

## Discussion

If the recipient is a child of a container view controller, this property holds the view controller it is contained in. If the recipient has no parent, the value in this property is `nil`.

Prior to iOS 5.0, if a view did not have a parent view controller and was being presented, the presenting view controller would be returned. On iOS 5, this behavior no longer occurs. Instead, use the presentingViewController property to access the presenting view controller.

## See Also

### Getting other related view controllers

var presentingViewController: UIViewController?

The view controller that presented this view controller.

var presentedViewController: UIViewController?

The view controller that is presented by this view controller, or one of its ancestors in the view controller hierarchy.

var splitViewController: UISplitViewController?

The nearest ancestor in the view controller hierarchy that is a split view controller.

var navigationController: UINavigationController?

The nearest ancestor in the view controller hierarchy that is a navigation controller.

var tabBarController: UITabBarController?

The nearest ancestor in the view controller hierarchy that is a tab bar controller.

