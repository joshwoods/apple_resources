

- UIKit
- UIViewController
-  presentedViewController 

Instance Property

# presentedViewController

The view controller that is presented by this view controller, or one of its ancestors in the view controller hierarchy.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var presentedViewController: UIViewController? { get }
```

## Discussion

When you present a view controller modally (either explicitly or implicitly) using the present(_:animated:completion:) method, the view controller that called the method has this property set to the view controller that it presented. If the current view controller did not present another view controller modally, the value in this property is `nil`.

## See Also

### Getting other related view controllers

var presentingViewController: UIViewController?

The view controller that presented this view controller.

var parent: UIViewController?

The parent view controller of the recipient.

var splitViewController: UISplitViewController?

The nearest ancestor in the view controller hierarchy that is a split view controller.

var navigationController: UINavigationController?

The nearest ancestor in the view controller hierarchy that is a navigation controller.

var tabBarController: UITabBarController?

The nearest ancestor in the view controller hierarchy that is a tab bar controller.

