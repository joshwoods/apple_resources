

- AppKit
- NSMenu
-  addItem(withTitle:action:keyEquivalent:) 

Instance Method

# addItem(withTitle:action:keyEquivalent:)

Creates a new menu item and adds it to the end of the menu.

macOS

``` source
func addItem(
    withTitle string: String,
    action selector: Selector?,
    keyEquivalent charCode: String
) -> NSMenuItem
```

## Parameters 

`string`  

A string to be made the title of the menu item.

`selector`  

The action-message selector to assign to the menu item.

`charCode`  

A string identifying the key to use as a key equivalent for the menu item. If you do not want the menu item to have a key equivalent, `keyEquiv` should be an empty string (`@""`) and not `nil`.

## Return Value

The created menu item (an object conforming to the NSMenuItem protocol) or `nil` if the object couldn’t be created.

## See Also

### Adding and Removing Menu Items

func insertItem(NSMenuItem, at: Int)

Inserts a menu item into the menu at a specific location.

func insertItem(withTitle: String, action: Selector?, keyEquivalent: String, at: Int) -> NSMenuItem

Creates and adds a menu item at a specified location in the menu.

func addItem(NSMenuItem)

Adds a menu item to the end of the menu.

func removeItem(NSMenuItem)

Removes a menu item from the menu.

func removeItem(at: Int)

Removes the menu item at a specified location in the menu.

func itemChanged(NSMenuItem)

Invoked when a menu item is modified visually (for example, its title changes).

func removeAllItems()

Removes all the menu items in the menu.

