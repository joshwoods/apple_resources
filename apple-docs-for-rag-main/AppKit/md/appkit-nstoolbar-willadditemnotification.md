

- AppKit
- NSToolbar
-  willAddItemNotification 

Type Property

# willAddItemNotification

Posts before the toolbar adds a new item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
class let willAddItemNotification: NSNotification.Name
```

## Discussion

The notification item is the `NSToolbar` object that’s about to add the item. The `userInfo` dictionary contains the following information:

| Key | Value |
|----|----|
| itemKey | The `NSToolbarItem` object being added. |

## See Also

### Related Documentation

func toolbarWillAddItem(Notification)

Tells the delegate that the toolbar is about to add the specified item.

### Managing items on the toolbar

var items: [NSToolbarItem]

An array containing the toolbar’s current items, in order.

var visibleItems: [NSToolbarItem]?

An array containing the toolbar’s currently visible items.

var centeredItemIdentifiers: Set&lt;NSToolbarItem.Identifier>

The set of custom items to display in the center of the toolbar.

var selectedItemIdentifier: NSToolbarItem.Identifier?

The identifier of the toolbar’s currently selected item.

class let didRemoveItemNotification: NSNotification.Name

Posted after an item is removed from a toolbar.

func insertItem(withItemIdentifier: NSToolbarItem.Identifier, at: Int)

Inserts an item into the toolbar at the specified index.

func removeItem(at: Int)

Removes the item at the specified index in the toolbar.

