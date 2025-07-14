

- UIKit
- UINavigationItem
-  trailingItemGroups 

Instance Property

# trailingItemGroups

Item groups to display in the trailing section of the navigation bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var trailingItemGroups: [UIBarButtonItemGroup] { get set }
```

## Discussion

Setting items through this property replaces the items you set through rightBarButtonItem or rightBarButtonItems.

## See Also

### Specifying custom views

var centerItemGroups: [UIBarButtonItemGroup]

Customizable item groups to display in the center section of the navigation bar.

var leadingItemGroups: [UIBarButtonItemGroup]

Item groups to display in the leading section of the navigation bar.

var pinnedTrailingGroup: UIBarButtonItemGroup?

The item group to display on the trailing edge of the navigation bar, on the trailing side of the overflow and search items.

var titleView: UIView?

A custom view that displays in the center of the navigation bar when the receiver is the top item.

var leftBarButtonItems: [UIBarButtonItem]?

An array of custom bar button items to display on the left (or leading) side of the navigation bar when the navigation item is the top item.

var leftBarButtonItem: UIBarButtonItem?

A custom bar button item that displays on the left (or leading) edge of the navigation bar when the navigation item is the top item.

var rightBarButtonItems: [UIBarButtonItem]?

An array of custom bar button items to display on the right (or trailing) side of the navigation bar when the navigation item is the top item.

var rightBarButtonItem: UIBarButtonItem?

A custom bar button item that displays on the right (or trailing) edge of the navigation bar when the navigation item is the top item.

func setLeftBarButtonItems([UIBarButtonItem]?, animated: Bool)

Sets the left bar button items, optionally animating the transition to the new items.

func setLeftBarButton(UIBarButtonItem?, animated: Bool)

Sets the custom bar button item, optionally animating the transition to the new item.

func setRightBarButtonItems([UIBarButtonItem]?, animated: Bool)

Sets the right bar button items, optionally animating the transition to the new items.

func setRightBarButton(UIBarButtonItem?, animated: Bool)

Sets the custom bar button item, optionally animating the transition to the view.

