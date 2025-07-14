

- UIKit
- UITabBarControllerDelegate
-  tabBarController(\_:shouldSelect:) 

Instance Method

# tabBarController(\_:shouldSelect:)

Asks the delegate whether the specified view controller should be made active.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    shouldSelect viewController: UIViewController
) -> Bool
```

## Parameters 

`tabBarController`  

The tab bar controller containing `viewController`.

`viewController`  

The view controller belonging to the tab that was tapped by the user.

## Return Value

true if the view controller’s tab should be selected or false if the current tab should remain active.

## Discussion

The tab bar controller calls this method in response to the user tapping a tab bar item. You can use this method to dynamically decide whether a given tab should be made the active tab.

## See Also

### Managing tab bar selections

func tabBarController(UITabBarController, didSelect: UIViewController)

Tells the delegate that the user selected an item in the tab bar.

