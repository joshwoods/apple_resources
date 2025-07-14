

- UIKit
- UITabBar
-  itemSpacing 

Instance Property

# itemSpacing

The amount of space (in points) to use between tab bar items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var itemSpacing: CGFloat { get set }
```

## Discussion

When the tab bar positions items using the UITabBar.ItemPositioning.centered option, it checks the value of this property to see if a custom spacing value has been supplied. The default value of this property is `0`, which causes the tab bar to use a system-defined default spacing value. Specifying a value greater than `0` causes the tab bar to use your custom value instead. If you try to set this property to a negative value, the tab bar sets the value to `0` instead.

## See Also

### Customizing item spacing

var itemPositioning: UITabBar.ItemPositioning

The positioning scheme for the tab bar items in the tab bar.

enum ItemPositioning

Constants that specify tab bar item positioning.

var itemWidth: CGFloat

The width (in points) of tab bar items.

