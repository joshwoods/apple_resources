

- AppKit
- NSToolbar
-  items 

Instance Property

# items

An array containing the toolbar’s current items, in order.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var items: [NSToolbarItem] { get }
```

## Discussion

To specify the default order of your toolbar’s items, implement the toolbarDefaultItemIdentifiers(_:) method in your toolbar delegate object. Use other methods of your delegate object to manage the placement of items in the toolbar.

## See Also

### Managing items on the toolbar

var visibleItems: [NSToolbarItem]?

An array containing the toolbar’s currently visible items.

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

