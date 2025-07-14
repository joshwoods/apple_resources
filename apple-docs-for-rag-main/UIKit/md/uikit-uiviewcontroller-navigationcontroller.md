

- UIKit
- UIViewController
-  navigationController 

Instance Property

# navigationController

The nearest ancestor in the view controller hierarchy that is a navigation controller.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var navigationController: UINavigationController? { get }
```

## Discussion

If the view controller or one of its ancestors is a child of a navigation controller, this property contains the owning navigation controller. This property is `nil` if the view controller is not embedded inside a navigation controller.

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

var tabBarController: UITabBarController?

The nearest ancestor in the view controller hierarchy that is a tab bar controller.

