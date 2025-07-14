

- UIKit
- UITabBarController
-  viewControllers 

Instance Property

# viewControllers

An array of the root view controllers displayed by the tab bar interface.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var viewControllers: [UIViewController]? { get set }
```

## Discussion

The default value of this property is `nil`. When configuring a tab bar controller, you can use this property to specify the content for each tab of the tab bar interface. The order of the view controllers in the array corresponds to the display order in the tab bar. Thus, the controller at index 0 corresponds to the left-most tab, the controller at index 1 the next tab to the right, and so on. If there are more view controllers than can fit in the tab bar, view controllers at the end of the array are managed by the More navigation controller, which is itself not included in this array.

Note

The More interface is not available in tvOS.

If you change the value of this property at runtime, the tab bar controller removes all of the old view controllers before installing the new ones. The tab bar items for the new view controllers are displayed immediately and are not animated into position. When changing the view controllers, the tab bar controller remembers the view controller object that was previously selected and attempts to reselect it. If the selected view controller is no longer present, it attempts to select the view controller at the same index in the array as the previous selection. If that index is invalid, it selects the view controller at index 0.

Setting this property also sets the customizableViewControllers property to the same set of view controllers.

## See Also

### Managing the view controllers

func setViewControllers([UIViewController]?, animated: Bool)

Sets the root view controllers of the tab bar controller.

var customizableViewControllers: [UIViewController]?

The subset of view controllers managed by this tab bar controller that can be customized.

var moreNavigationController: UINavigationController

The view controller that manages the More navigation interface.

