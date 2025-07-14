

- AppKit
- NSToolbarItem
-  itemIdentifier 

Instance Property

# itemIdentifier

The value you use to identify the toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var itemIdentifier: NSToolbarItem.Identifier { get }
```

## Discussion

Use this property to distinguish one toolbar item from another on the same toolbar.

## See Also

### Related Documentation

init(itemIdentifier: NSToolbarItem.Identifier)

Creates a toolbar item with the specified identifier.

### Getting the toolbar item’s identity

struct Identifier

Constants for the standard toolbar items that the system provides.

