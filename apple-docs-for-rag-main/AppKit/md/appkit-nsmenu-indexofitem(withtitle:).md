

- AppKit
- NSMenu
-  indexOfItem(withTitle:) 

Instance Method

# indexOfItem(withTitle:)

Returns the index of the first menu item in the menu that has a specified title.

macOS

``` source
func indexOfItem(withTitle title: String) -> Int
```

## Parameters 

`title`  

The title of a menu item in the menu.

## Return Value

The integer index of the menu item or, if no such menu item is in the menu, –1.

## See Also

### Related Documentation

func item(at: Int) -> NSMenuItem?

Returns the menu item at a specific location of the menu.

func item(withTitle: String) -> NSMenuItem?

Returns the first menu item in the menu with a specified title.

func insertItem(NSMenuItem, at: Int)

Inserts a menu item into the menu at a specific location.

### Finding Indices of Menu Items

func index(of: NSMenuItem) -> Int

Returns the index identifying the location of a specified menu item in the menu.

func indexOfItem(withTag: Int) -> Int

Returns the index of the first menu item in the menu identified by a tag.

func indexOfItem(withTarget: Any?, andAction: Selector?) -> Int

Returns the index of the first menu item in the menu that has a specified action and target.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the first menu item in the menu that has a given represented object.

func indexOfItem(withSubmenu: NSMenu?) -> Int

Returns the index of the menu item in the menu with the given submenu.

