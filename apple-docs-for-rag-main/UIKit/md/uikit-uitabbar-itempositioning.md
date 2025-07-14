

- UIKit
- UITabBar
-  itemPositioning 

Instance Property

# itemPositioning

The positioning scheme for the tab bar items in the tab bar.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var itemPositioning: UITabBar.ItemPositioning { get set }
```

## Discussion

The default value for this property, UITabBar.ItemPositioning.automatic, results in the default tab bar item positioning according to the current environment:

- In a horizontally compact environment, the tab bar spreads items across the entire space, adjusting inter-item spacing as needed.

- In a horizontally regular environment, the tab bar uses the itemWidth and itemSpacing properties to set the width of items and the spacing between items, positioning those items in the center of the available space. This configuration has the potential to leave space along the left and right edges of the tab bar.

You can force a specific positioning scheme by changing the value of this property to a different value. For a list of possible values, see the constant descriptions for the UITabBar.ItemPositioning type.

## See Also

### Customizing item spacing

enum ItemPositioning

Constants that specify tab bar item positioning.

var itemSpacing: CGFloat

The amount of space (in points) to use between tab bar items.

var itemWidth: CGFloat

The width (in points) of tab bar items.

