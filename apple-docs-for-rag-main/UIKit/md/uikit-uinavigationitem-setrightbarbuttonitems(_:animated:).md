

- UIKit
- UINavigationItem
-  setRightBarButtonItems(\_:animated:) 

Instance Method

# setRightBarButtonItems(\_:animated:)

Sets the right bar button items, optionally animating the transition to the new items.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setRightBarButtonItems(
    _ items: [UIBarButtonItem]?,
    animated: Bool
)
```

## Parameters 

`items`  

An array of custom bar button items to display on the right side of the navigation bar.

`animated`  

Specify true to animate the transition to the custom bar items when this item is the top item. Specify false to set the items immediately without animating the change.

## Discussion

If two navigation items have the same custom left or right bar button items, those bar button items remain stationary during the transition when the navigation item is pushed or popped.

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

var rightBarButtonItems: [UIBarButtonItem]?

An array of custom bar button items to display on the right (or trailing) side of the navigation bar when the navigation item is the top item.

var rightBarButtonItem: UIBarButtonItem?

A custom bar button item that displays on the right (or trailing) edge of the navigation bar when the navigation item is the top item.

func setLeftBarButtonItems([UIBarButtonItem]?, animated: Bool)

Sets the left bar button items, optionally animating the transition to the new items.

func setLeftBarButton(UIBarButtonItem?, animated: Bool)

Sets the custom bar button item, optionally animating the transition to the new item.

func setRightBarButton(UIBarButtonItem?, animated: Bool)

Sets the custom bar button item, optionally animating the transition to the view.

