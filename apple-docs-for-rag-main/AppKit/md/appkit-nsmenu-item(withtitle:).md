

- AppKit
- NSMenu
-  item(withTitle:) 

Instance Method

# item(withTitle:)

Returns the first menu item in the menu with a specified title.

macOS

``` source
func item(withTitle title: String) -> NSMenuItem?
```

## Parameters 

`title`  

The title of a menu item.

## Return Value

The found menu item (an object conforming to the NSMenuItem protocol) or `nil` if the object couldn’t be found.

## See Also

### Related Documentation

func indexOfItem(withTitle: String) -> Int

Returns the index of the first menu item in the menu that has a specified title.

### Finding Menu Items

func item(withTag: Int) -> NSMenuItem?

Returns the first menu item in the menu with the specified tag.

func item(at: Int) -> NSMenuItem?

Returns the menu item at a specific location of the menu.

var numberOfItems: Int

The number of menu items in the menu, including separator items.

var items: [NSMenuItem]

An array containing the menu items in the menu.

