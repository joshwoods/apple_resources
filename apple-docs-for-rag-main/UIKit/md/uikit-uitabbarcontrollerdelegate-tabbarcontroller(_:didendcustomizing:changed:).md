

- UIKit
- UITabBarControllerDelegate
-  tabBarController(\_:didEndCustomizing:changed:) 

Instance Method

# tabBarController(\_:didEndCustomizing:changed:)

Tells the delegate that the tab bar customization sheet was dismissed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    didEndCustomizing viewControllers: [UIViewController],
    changed: Bool
)
```

## Parameters 

`tabBarController`  

The tab bar controller that is being customized.

`viewControllers`  

The view controllers of the tab bar controller. The arrangement of the controllers in the array represents the new display order within the tab bar.

`changed`  

A Boolean value indicating whether items changed on the tab bar. true if items changed or false if they did not.

## Discussion

You can use this method to respond to changes to the order of tabs in the tab bar.

## See Also

### Managing tab bar customizations

func tabBarController(UITabBarController, willBeginCustomizing: [UIViewController])

Tells the delegate that the tab bar customization sheet is about to be displayed.

func tabBarController(UITabBarController, willEndCustomizing: [UIViewController], changed: Bool)

Tells the delegate that the tab bar customization sheet is about to be dismissed.

