

- UIKit
- UINavigationItem
-  rightBarButtonItems 

Instance Property

# rightBarButtonItems

An array of custom bar button items to display on the right (or trailing) side of the navigation bar when the navigation item is the top item.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var rightBarButtonItems: [UIBarButtonItem]? { get set }
```

## Discussion

This array can contain 0 or more bar button items to display on the right (or trailing) side of the navigation bar. Items are displayed right-to-left in the same order as they appear in the array. Thus, the first item in the array is the rightmost item and other items are added to the left of the previous item. In a right-to-left user interface, the items are automatically flipped.

If there is not enough room to display all of the items in the array, those that would overlap the title view (if present) or the buttons on the left side of the bar are not displayed.

The first item in the array can also be set using the rightBarButtonItem property.

## See Also

### Specifying custom views

var centerItemGroups: [UIBarButtonItemGroup]

Customizable item groups to display in the center section of the navigation bar.

var leadingItemGroups: [UIBarButtonItemGroup]

Item groups to display in the leading section of the navigation bar.

var trailingItemGroups: [UIBarButtonItemGroup]

Item groups to display in the trailing section of the navigation bar.

var pinnedTrailingGroup: UIBarButtonItemGroup?

The item group to display on the trailing edge of the navigation bar, on the trailing side of the overflow and search items.

var titleView: UIView?

A custom view that displays in the center of the navigation bar when the receiver is the top item.

var leftBarButtonItems: [UIBarButtonItem]?

An array of custom bar button items to display on the left (or leading) side of the navigation bar when the navigation item is the top item.

var leftBarButtonItem: UIBarButtonItem?

A custom bar button item that displays on the left (or leading) edge of the navigation bar when the navigation item is the top item.

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

