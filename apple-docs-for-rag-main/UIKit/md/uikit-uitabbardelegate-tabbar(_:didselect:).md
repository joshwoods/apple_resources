

- UIKit
- UITabBarDelegate
-  tabBar(\_:didSelect:) 

Instance Method

# tabBar(\_:didSelect:)

Sent to the delegate when the user selects a tab bar item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tabBar(
    _ tabBar: UITabBar,
    didSelect item: UITabBarItem
)
```

## Parameters 

`tabBar`  

The tab bar that is being customized.

`item`  

The tab bar item that was selected.

## See Also

### Customizing tab bars

func tabBar(UITabBar, willBeginCustomizing: [UITabBarItem])

Sent to the delegate before the customizing modal view is displayed.

func tabBar(UITabBar, didBeginCustomizing: [UITabBarItem])

Sent to the delegate after the customizing modal view is displayed.

func tabBar(UITabBar, willEndCustomizing: [UITabBarItem], changed: Bool)

Sent to the delegate before the customizing modal view is dismissed.

func tabBar(UITabBar, didEndCustomizing: [UITabBarItem], changed: Bool)

Sent to the delegate after the customizing modal view is dismissed.

