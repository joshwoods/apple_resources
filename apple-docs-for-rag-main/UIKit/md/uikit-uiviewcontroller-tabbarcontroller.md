

- UIKit
- UIViewController
-  tabBarController 

Instance Property

# tabBarController

The nearest ancestor in the view controller hierarchy that is a tab bar controller.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var tabBarController: UITabBarController? { get }
```

## Discussion

If the view controller or one of its ancestors is a child of a tab bar controller, this property contains the owning tab bar controller. This property is `nil` if the view controller is not embedded inside a tab bar controller.

## See Also

### Getting other related view controllers

var presentingViewController: UIViewController?

The view controller that presented this view controller.

var presentedViewController: UIViewController?

The view controller that is presented by this view controller, or one of its ancestors in the view controller hierarchy.

var parent: UIViewController?

The parent view controller of the recipient.

var splitViewController: UISplitViewController?

The nearest ancestor in the view controller hierarchy that is a split view controller.

var navigationController: UINavigationController?

The nearest ancestor in the view controller hierarchy that is a navigation controller.

