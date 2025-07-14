

- UIKit
- UITabBarControllerDelegate
-  tabBarController(\_:willBeginCustomizing:) 

Instance Method

# tabBarController(\_:willBeginCustomizing:)

Tells the delegate that the tab bar customization sheet is about to be displayed.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    willBeginCustomizing viewControllers: [UIViewController]
)
```

## Parameters 

`tabBarController`  

The tab bar controller that is being customized.

`viewControllers`  

The view controllers to be displayed in the customization sheet. This list typically contains all custom view controllers you added but does not include some standard controllers, such as the one that manages the More tab.

## See Also

### Managing tab bar customizations

func tabBarController(UITabBarController, willEndCustomizing: [UIViewController], changed: Bool)

Tells the delegate that the tab bar customization sheet is about to be dismissed.

func tabBarController(UITabBarController, didEndCustomizing: [UIViewController], changed: Bool)

Tells the delegate that the tab bar customization sheet was dismissed.

