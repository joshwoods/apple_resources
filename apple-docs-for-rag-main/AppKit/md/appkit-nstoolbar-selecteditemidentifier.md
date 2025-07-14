

- AppKit
- NSToolbar
-  selectedItemIdentifier 

Instance Property

# selectedItemIdentifier

The identifier of the toolbar’s currently selected item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var selectedItemIdentifier: NSToolbarItem.Identifier? { get set }
```

## Discussion

The value of this property is `nil` if the toolbar doesn’t have a selected item.

## See Also

### Managing items on the toolbar

var items: [NSToolbarItem]

An array containing the toolbar’s current items, in order.

var visibleItems: [NSToolbarItem]?

An array containing the toolbar’s currently visible items.

var centeredItemIdentifiers: Set&lt;NSToolbarItem.Identifier>

The set of custom items to display in the center of the toolbar.

class let willAddItemNotification: NSNotification.Name

Posts before the toolbar adds a new item.

class let didRemoveItemNotification: NSNotification.Name

Posted after an item is removed from a toolbar.

func insertItem(withItemIdentifier: NSToolbarItem.Identifier, at: Int)

Inserts an item into the toolbar at the specified index.

func removeItem(at: Int)

Removes the item at the specified index in the toolbar.

