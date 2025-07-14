

- AppKit
- NSWindowTabGroup
-  isTabBarVisible 

Instance Property

# isTabBarVisible

A Boolean value indicating whether the tabbed window group currently displays a tab bar.

macOS 10.13+

``` source
var isTabBarVisible: Bool { get }
```

## Discussion

Typically, a tabbed window displays a tab bar if there is more than one window in the tabbing group. The tab bar can also be manually toggled using the toggleTabBar(_:) method.

## See Also

### Configuring the Tab User Interface

var isOverviewVisible: Bool

A Boolean value indicating if the tab overview is currently displayed.

