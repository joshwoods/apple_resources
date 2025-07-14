

- UIKit
- UITabBarController
-  tabBar 

Instance Property

# tabBar

The tab bar view associated with this controller.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var tabBar: UITabBar { get }
```

## Discussion

You should never attempt to manipulate the UITabBar object itself stored in this property. If you attempt to do so, the tab bar view throws an exception. To configure the items for your tab bar interface, you should instead assign one or more custom view controllers to the viewControllers property. The tab bar collects the needed tab bar items from the view controllers you specify.

The tab bar view provided by this property is only for situations where you want to display an action sheet using the show(from:) method of the UIActionSheet class.

