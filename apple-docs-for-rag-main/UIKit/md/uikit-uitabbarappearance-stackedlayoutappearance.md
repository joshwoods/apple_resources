

- UIKit
- UITabBarAppearance
-  stackedLayoutAppearance 

Instance Property

# stackedLayoutAppearance

The appearance attributes for items with a stacked layout.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var stackedLayoutAppearance: UITabBarItemAppearance { get set }
```

## Discussion

If you didn’t provide a set of explicit attributes at initialization time, UIKit provides an object with default attributes.

## See Also

### Configuring stacked item appearances

var stackedItemPositioning: UITabBar.ItemPositioning

The scheme to use when positioning stacked items within the tab bar.

var stackedItemSpacing: CGFloat

The amount of space to insert between stacked tab bar items.

var stackedItemWidth: CGFloat

The width of stacked items in the tab bar.

