

- UIKit
- UITabBarControllerDelegate
-  tabBarController(\_:willEndCustomizing:changed:) 

Instance Method

# tabBarController(\_:willEndCustomizing:changed:)

Tells the delegate that the tab bar customization sheet is about to be dismissed.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    willEndCustomizing viewControllers: [UIViewController],
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

This method is called in response to the user tapping the Done button on the sheet but before the sheet is dismissed.

## See Also

### Managing tab bar customizations

func tabBarController(UITabBarController, willBeginCustomizing: [UIViewController])

Tells the delegate that the tab bar customization sheet is about to be displayed.

func tabBarController(UITabBarController, didEndCustomizing: [UIViewController], changed: Bool)

Tells the delegate that the tab bar customization sheet was dismissed.

