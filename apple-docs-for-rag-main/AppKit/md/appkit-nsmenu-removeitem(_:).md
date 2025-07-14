

- AppKit
- NSMenu
-  removeItem(\_:) 

Instance Method

# removeItem(\_:)

Removes a menu item from the menu.

macOS

``` source
func removeItem(_ item: NSMenuItem)
```

## Parameters 

`item`  

The menu item to remove.

## See Also

### Adding and Removing Menu Items

func insertItem(NSMenuItem, at: Int)

Inserts a menu item into the menu at a specific location.

func insertItem(withTitle: String, action: Selector?, keyEquivalent: String, at: Int) -> NSMenuItem

Creates and adds a menu item at a specified location in the menu.

func addItem(NSMenuItem)

Adds a menu item to the end of the menu.

func addItem(withTitle: String, action: Selector?, keyEquivalent: String) -> NSMenuItem

Creates a new menu item and adds it to the end of the menu.

func removeItem(at: Int)

Removes the menu item at a specified location in the menu.

func itemChanged(NSMenuItem)

Invoked when a menu item is modified visually (for example, its title changes).

func removeAllItems()

Removes all the menu items in the menu.

