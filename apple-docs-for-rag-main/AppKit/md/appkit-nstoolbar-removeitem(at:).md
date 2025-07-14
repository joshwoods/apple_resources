

- AppKit
- NSToolbar
-  removeItem(at:) 

Instance Method

# removeItem(at:)

Removes the item at the specified index in the toolbar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
func removeItem(at index: Int)
```

## Parameters 

`index`  

The index of the item to remove.

## Discussion

Typically, you don’t call this method directly from your code. Instead, you specify your toolbar’s allowed items, and the set of default items you want to appear. After that, you let the user customize the toolbar.

Any changes you make to the toolbar appear in all NSToolbar objects with the same identifier value. This method does not trigger a call to your delegate’s toolbar(_:itemIdentifier:canBeInsertedAt:) method for the removal of the item.

## See Also

### Managing items on the toolbar

var items: [NSToolbarItem]

An array containing the toolbar’s current items, in order.

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

