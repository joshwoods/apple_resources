

- UIKit
- UIViewController
-  presentingViewController 

Instance Property

# presentingViewController

The view controller that presented this view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var presentingViewController: UIViewController? { get }
```

## Discussion

When you present a view controller modally (either explicitly or implicitly) using the present(_:animated:completion:) method, the view controller that was presented has this property set to the view controller that presented it. If the view controller was not presented modally, but one of its ancestors was, this property contains the view controller that presented the ancestor. If neither the current view controller or any of its ancestors were presented modally, the value in this property is `nil`.

## See Also

### Getting other related view controllers

var presentedViewController: UIViewController?

The view controller that is presented by this view controller, or one of its ancestors in the view controller hierarchy.

var parent: UIViewController?

The parent view controller of the recipient.

var splitViewController: UISplitViewController?

The nearest ancestor in the view controller hierarchy that is a split view controller.

var navigationController: UINavigationController?

The nearest ancestor in the view controller hierarchy that is a navigation controller.

var tabBarController: UITabBarController?

The nearest ancestor in the view controller hierarchy that is a tab bar controller.

