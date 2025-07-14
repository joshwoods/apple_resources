

- AppKit
- NSMenu
-  addItem(\_:) 

Instance Method

# addItem(\_:)

Adds a menu item to the end of the menu.

macOS

``` source
func addItem(_ newItem: NSMenuItem)
```

## Parameters 

`newItem`  

The menu item (an object conforming to the NSMenuItem protocol) to add to the menu.

## Discussion

This method invokes insertItem(_:at:). Thus, the menu does not accept the menu item if it already belongs to another menu. After adding the menu item, the menu updates itself.

## See Also

### Adding and Removing Menu Items

func insertItem(NSMenuItem, at: Int)

Inserts a menu item into the menu at a specific location.

func insertItem(withTitle: String, action: Selector?, keyEquivalent: String, at: Int) -> NSMenuItem

Creates and adds a menu item at a specified location in the menu.

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

