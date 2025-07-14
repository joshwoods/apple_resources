

- UIKit
- UITabBarAppearance
-  stackedItemPositioning 

Instance Property

# stackedItemPositioning

The scheme to use when positioning stacked items within the tab bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var stackedItemPositioning: UITabBar.ItemPositioning { get set }
```

## Discussion

Use this property to specify whether you want the items centered in the available space or distributed across the entire width of the tab bar.

## See Also

### Configuring stacked item appearances

var stackedLayoutAppearance: UITabBarItemAppearance

The appearance attributes for items with a stacked layout.

var stackedItemSpacing: CGFloat

The amount of space to insert between stacked tab bar items.

var stackedItemWidth: CGFloat

The width of stacked items in the tab bar.

