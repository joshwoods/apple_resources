

- AppKit
- NSToolbarItem
-  init(itemIdentifier:barButtonItem:) 

Initializer

# init(itemIdentifier:barButtonItem:)

Creates a toolbar item with property values from the specified bar button item.

Mac Catalyst 13.0+

``` source
@MainActor
convenience init(
    itemIdentifier: NSToolbarItem.Identifier,
    barButtonItem: UIBarButtonItem
)
```

## Parameters 

`itemIdentifier`  

The identifier for the toolbar item. You use this value to identify the item within your app, so you don’t need to localize it. For example, your toolbar delegate uses this value to identify the specific toolbar item.

`barButtonItem`  

The bar button item to use to create the toolbar item.

## Return Value

A new toolbar item.

## Discussion

Use this method to create and initialize a toolbar item with property values from a UIBarButtonItem, such as title, image, action, and target.

Note

In macOS 12 and earlier, this method doesn’t support creating a toolbar item from a bar button item that contains a custom view.

## See Also

### Creating a toolbar item

init(itemIdentifier: NSToolbarItem.Identifier)

Creates a toolbar item with the specified identifier.

