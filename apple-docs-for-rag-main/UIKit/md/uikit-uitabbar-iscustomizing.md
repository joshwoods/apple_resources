

- UIKit
- UITabBar
-  isCustomizing 

Instance Property

# isCustomizing

A Boolean value indicating whether the user is currently customizing the tab bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
@MainActor
var isCustomizing: Bool { get }
```

## See Also

### Supporting user customization of tab bars

func beginCustomizingItems([UITabBarItem])

Presents a standard interface that lets the user customize the contents of the tab bar.

func endCustomizing(animated: Bool) -> Bool

Dismisses the standard interface used to customize the tab bar.

