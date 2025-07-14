

- UIKit
- UITabBarControllerDelegate
-  tabBarController(\_:didSelect:) 

Instance Method

# tabBarController(\_:didSelect:)

Tells the delegate that the user selected an item in the tab bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    didSelect viewController: UIViewController
)
```

## Parameters 

`tabBarController`  

The tab bar controller containing `viewController`.

`viewController`  

The view controller that the user selected. In iOS v3.0 and later, this could be the same view controller that was already selected.

## Discussion

In iOS v3.0 and later, the tab bar controller calls this method regardless of whether the selected view controller changed. In addition, it is called only in response to user taps in the tab bar and is not called when your code changes the tab bar contents programmatically.

In versions of iOS prior to version 3.0, this method is called only when the selected view controller actually changes. In other words, it is not called when the same view controller is selected. In addition, the method was called for both programmatic and user-initiated changes to the selected view controller.

## See Also

### Managing tab bar selections

func tabBarController(UITabBarController, shouldSelect: UIViewController) -> Bool

Asks the delegate whether the specified view controller should be made active.

