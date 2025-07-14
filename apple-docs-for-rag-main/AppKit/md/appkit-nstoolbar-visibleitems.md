

- AppKit
- NSToolbar
-  visibleItems 

Instance Property

# visibleItems

An array containing the toolbar’s currently visible items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var visibleItems: [NSToolbarItem]? { get }
```

## Discussion

This property doesn’t contain items in the overflow menu because those items aren’t visible.

## See Also

### Managing items on the toolbar

var items: [NSToolbarItem]

An array containing the toolbar’s current items, in order.

var centeredItemIdentifiers: Set&lt;NSToolbarItem.Identifier>

The set of custom items to display in the center of the toolbar.

var selectedItemIdentifier: NSToolbarItem.Identifier?

The identifier of the toolbar’s currently selected item.

class let willAddItemNotification: NSNotification.Name

Posts before the toolbar adds a new item.

class let didRemoveItemNotification: NSNotification.Name

Posted after an item is removed from a toolbar.

func insertItem(withItemIdentifier: NSToolbarItem.Identifier, at: Int)

Inserts an item into the toolbar at the specified index.

func removeItem(at: Int)

Removes the item at the specified index in the toolbar.

