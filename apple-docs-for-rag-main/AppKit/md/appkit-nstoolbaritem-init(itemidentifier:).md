

- AppKit
- NSToolbarItem
-  init(itemIdentifier:) 

Initializer

# init(itemIdentifier:)

Creates a toolbar item with the specified identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
init(itemIdentifier: NSToolbarItem.Identifier)
```

## Parameters 

`itemIdentifier`  

The identifier for the toolbar item. You use this value to identify the item within your app, so you don’t need to localize it. For example, your toolbar delegate uses this value to identify the specific toolbar item.

## Return Value

A new toolbar item.

## See Also

### Related Documentation

Toolbar Programming Topics for Cocoa

### Creating a toolbar item

convenience init(itemIdentifier: NSToolbarItem.Identifier, barButtonItem: UIBarButtonItem)

Creates a toolbar item with property values from the specified bar button item.

