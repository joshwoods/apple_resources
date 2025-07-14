

- UIKit
- UINavigationItem
-  titleView 

Instance Property

# titleView

A custom view that displays in the center of the navigation bar when the receiver is the top item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var titleView: UIView? { get set }
```

## Discussion

If this property value is `nil`, the navigation item’s title is displayed in the center of the navigation bar when the receiver is the top item. If you set this property to a custom title, it is displayed instead of the title.

Custom views can contain buttons. Use the init(type:) method in UIButton class to add buttons to your custom view in the style of the navigation bar. Custom title views are centered on the navigation bar and may be resized to fit.

The default value is `nil`.

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

