

- UIKit
- UINavigationItem
-  centerItemGroups 

Instance Property

# centerItemGroups

Customizable item groups to display in the center section of the navigation bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var centerItemGroups: [UIBarButtonItemGroup] { get set }
```

## Mentioned in 

Building a desktop-class iPad app

## Discussion

Use this property to specify *center item groups*, groups of controls that appear in the navigation bar to provide quick access to your app’s capabilities. Center items appear in the center of the navigation bar for the UINavigationItem.ItemStyle.browser and UINavigationItem.ItemStyle.editor styles, and in the overflow menu for the UINavigationItem.ItemStyle.navigator style.

Optionally, you can allow people to customize the layout of center item groups and preserve that customization across app launches. When you create center item groups, you can choose from three types of behaviors:

- Create a fixed group to disallow moving or removing that group from the navigation bar.

- Create a movable group to allow moving a group in the navigation bar, but not removing it.

- Create an optional group to allow moving, removing, or adding back that group.

The following code enables center item layout customization by assigning a customizationIdentifier. Then, it shows two approaches to creating center item groups: creating a group from an array of items and creating a group from a single item.

```
// Specify a unique customization identifier to enable navigation bar layout customization.
navigationItem.customizationIdentifier = "MyCustomNavigationItem"

// Create a fixed group with multiple items.
let editingGroup = UIBarButtonItemGroup.fixedGroup(items: [
    UIBarButtonItem(title: "Undo", image: UIImage(systemName: "arrow.uturn.backward"), primaryAction: UIAction { _ in
        // Implement undo action.
    }),
    UIBarButtonItem(title: "Redo", image: UIImage(systemName: "arrow.uturn.forward"), primaryAction: UIAction { _ in
        // Implement redo action.
    })
])

// Create a movable group from a single item.
let croppingItem = UIBarButtonItem(title: "Crop", image: UIImage(systemName: "crop"), primaryAction: UIAction { _ in
    // Implement crop action.
})
let croppingGroup = croppingItem.creatingMovableGroup(customizationIdentifier: "Cropping")

navigationItem.centerItemGroups = [editingGroup, croppingGroup]
```

## See Also

### Specifying custom views

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

func setRightBarButtonItems([UIBarButtonItem]?, animated: Bool)

Sets the right bar button items, optionally animating the transition to the new items.

func setRightBarButton(UIBarButtonItem?, animated: Bool)

Sets the custom bar button item, optionally animating the transition to the view.

