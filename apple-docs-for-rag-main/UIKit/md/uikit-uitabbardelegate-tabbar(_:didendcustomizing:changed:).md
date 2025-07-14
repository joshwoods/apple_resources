

- UIKit
- UITabBarDelegate
-  tabBar(\_:didEndCustomizing:changed:) 

Instance Method

# tabBar(\_:didEndCustomizing:changed:)

Sent to the delegate after the customizing modal view is dismissed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
@MainActor
optional func tabBar(
    _ tabBar: UITabBar,
    didEndCustomizing items: [UITabBarItem],
    changed: Bool
)
```

## Parameters 

`tabBar`  

The tab bar that is being customized.

`items`  

The items on the customizing modal view.

`changed`  

true if the visible set of items on the tab bar changed; otherwise, false.

## See Also

### Customizing tab bars

func tabBar(UITabBar, willBeginCustomizing: [UITabBarItem])

Sent to the delegate before the customizing modal view is displayed.

func tabBar(UITabBar, didBeginCustomizing: [UITabBarItem])

Sent to the delegate after the customizing modal view is displayed.

func tabBar(UITabBar, willEndCustomizing: [UITabBarItem], changed: Bool)

Sent to the delegate before the customizing modal view is dismissed.

func tabBar(UITabBar, didSelect: UITabBarItem)

Sent to the delegate when the user selects a tab bar item.

