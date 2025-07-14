

- UIKit
- UITabBarDelegate
-  tabBar(\_:willBeginCustomizing:) 

Instance Method

# tabBar(\_:willBeginCustomizing:)

Sent to the delegate before the customizing modal view is displayed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
@MainActor
optional func tabBar(
    _ tabBar: UITabBar,
    willBeginCustomizing items: [UITabBarItem]
)
```

## Parameters 

`tabBar`  

The tab bar that is being customized.

`items`  

The items on the customizing modal view.

## Discussion

Use the beginCustomizingItems(_:) method of UITabBar to display the customizing modal view and begin the customizing mode.

## See Also

### Customizing tab bars

func tabBar(UITabBar, didBeginCustomizing: [UITabBarItem])

Sent to the delegate after the customizing modal view is displayed.

func tabBar(UITabBar, willEndCustomizing: [UITabBarItem], changed: Bool)

Sent to the delegate before the customizing modal view is dismissed.

func tabBar(UITabBar, didEndCustomizing: [UITabBarItem], changed: Bool)

Sent to the delegate after the customizing modal view is dismissed.

func tabBar(UITabBar, didSelect: UITabBarItem)

Sent to the delegate when the user selects a tab bar item.

