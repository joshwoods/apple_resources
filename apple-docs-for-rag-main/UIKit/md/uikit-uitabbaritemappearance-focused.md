

- UIKit
- UITabBarItemAppearance
-  focused 

Instance Property

# focused

The appearance data to apply to the tab bar item when it’s focused.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var focused: UITabBarItemStateAppearance { get }
```

## Discussion

To set the attributes for this state, get the object in this property and modify it.

## See Also

### Configuring attributes for different item states

var normal: UITabBarItemStateAppearance

The appearance data to apply to the tab bar item when it’s enabled, unselected, and not the focused item.

var selected: UITabBarItemStateAppearance

The appearance data to apply to the tab bar item when it’s selected.

var disabled: UITabBarItemStateAppearance

The appearance data to apply to the tab bar item when it’s disabled.

