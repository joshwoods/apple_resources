

- AppKit
- NSToolbar
-  centeredItemIdentifiers 

Instance Property

# centeredItemIdentifiers

The set of custom items to display in the center of the toolbar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+

``` source
@MainActor
var centeredItemIdentifiers: Set { get set }
```

## Discussion

Set this property to the items you want to appear together in the center of the toolbar. Specify the initial order of the items using the toolbarDefaultItemIdentifiers(_:) method of your toolbar delegate object.

## See Also

### Managing items on the toolbar

var items: [NSToolbarItem]

An array containing the toolbar’s current items, in order.

var visibleItems: [NSToolbarItem]?

An array containing the toolbar’s currently visible items.

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

