

- AppKit
- NSToolbar
-  didRemoveItemNotification 

Type Property

# didRemoveItemNotification

Posted after an item is removed from a toolbar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
class let didRemoveItemNotification: NSNotification.Name
```

## Discussion

The notification item is the `NSToolbar` object that removed the item. The `userInfo` dictionary contains the following information:

| Key | Value |
|----|----|
| itemKey | The `NSToolbarItem` object that was removed. |

## See Also

### Related Documentation

func toolbarDidRemoveItem(Notification)

Tells the delegate that the toolbar removed the specified item.

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

func insertItem(withItemIdentifier: NSToolbarItem.Identifier, at: Int)

Inserts an item into the toolbar at the specified index.

func removeItem(at: Int)

Removes the item at the specified index in the toolbar.

