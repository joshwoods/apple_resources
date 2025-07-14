

- AppKit
- NSMenu
-  insertItem(\_:at:) 

Instance Method

# insertItem(\_:at:)

Inserts a menu item into the menu at a specific location.

macOS

``` source
func insertItem(
    _ newItem: NSMenuItem,
    at index: Int
)
```

## Parameters 

`newItem`  

An object conforming to the `NSMenuItem` protocol that represents a menu item.

`index`  

An integer index identifying the location of the menu item in the menu.

## Discussion

This method posts an didAddItemNotification, allowing interested observers to update as appropriate. This method is a primitive method. All item-addition methods end up calling this method, so this is where you should implement custom behavior on adding new items to a menu in a custom subclass. If the menu item already exists in another menu, it is not inserted and the method raises an exception of type internalInconsistencyException.

## See Also

### Related Documentation

func item(at: Int) -> NSMenuItem?

Returns the menu item at a specific location of the menu.

### Adding and Removing Menu Items

func insertItem(withTitle: String, action: Selector?, keyEquivalent: String, at: Int) -> NSMenuItem

Creates and adds a menu item at a specified location in the menu.

func addItem(NSMenuItem)

Adds a menu item to the end of the menu.

func addItem(withTitle: String, action: Selector?, keyEquivalent: String) -> NSMenuItem

Creates a new menu item and adds it to the end of the menu.

func removeItem(NSMenuItem)

Removes a menu item from the menu.

func removeItem(at: Int)

Removes the menu item at a specified location in the menu.

func itemChanged(NSMenuItem)

Invoked when a menu item is modified visually (for example, its title changes).

func removeAllItems()

Removes all the menu items in the menu.

