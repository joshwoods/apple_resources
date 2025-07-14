

- AppKit
- NSMenu
-  indexOfItem(withTarget:andAction:) 

Instance Method

# indexOfItem(withTarget:andAction:)

Returns the index of the first menu item in the menu that has a specified action and target.

macOS

``` source
func indexOfItem(
    withTarget target: Any?,
    andAction actionSelector: Selector?
) -> Int
```

## Parameters 

`target`  

An object that is set as the target of a menu item of the menu.

`actionSelector`  

A selector identifying an action method. If `actionSelector` is `NULL`, the first menu item in the menu that has target `anObject` is returned.

## Return Value

The integer index of the menu item or, if no such menu item is in the menu, –1.

## See Also

### Related Documentation

func item(at: Int) -> NSMenuItem?

Returns the menu item at a specific location of the menu.

func insertItem(NSMenuItem, at: Int)

Inserts a menu item into the menu at a specific location.

### Finding Indices of Menu Items

func index(of: NSMenuItem) -> Int

Returns the index identifying the location of a specified menu item in the menu.

func indexOfItem(withTitle: String) -> Int

Returns the index of the first menu item in the menu that has a specified title.

func indexOfItem(withTag: Int) -> Int

Returns the index of the first menu item in the menu identified by a tag.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the first menu item in the menu that has a given represented object.

func indexOfItem(withSubmenu: NSMenu?) -> Int

Returns the index of the menu item in the menu with the given submenu.

