

- AppKit
- NSMenu
-  item(withTag:) 

Instance Method

# item(withTag:)

Returns the first menu item in the menu with the specified tag.

macOS

``` source
func item(withTag tag: Int) -> NSMenuItem?
```

## Parameters 

`tag`  

A numeric tag associated with a menu item.

## Return Value

The found menu item (an object conforming to the NSMenuItem protocol) or `nil` if the object couldn’t be found.

## See Also

### Related Documentation

func indexOfItem(withTag: Int) -> Int

Returns the index of the first menu item in the menu identified by a tag.

### Finding Menu Items

func item(withTitle: String) -> NSMenuItem?

Returns the first menu item in the menu with a specified title.

func item(at: Int) -> NSMenuItem?

Returns the menu item at a specific location of the menu.

var numberOfItems: Int

The number of menu items in the menu, including separator items.

var items: [NSMenuItem]

An array containing the menu items in the menu.

