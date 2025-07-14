

- AppKit
- NSMenu
-  items 

Instance Property

# items

An array containing the menu items in the menu.

macOS

``` source
var items: [NSMenuItem] { get set }
```

## Discussion

This property contains an array of menu items in the menu.

## See Also

### Finding Menu Items

func item(withTag: Int) -> NSMenuItem?

Returns the first menu item in the menu with the specified tag.

func item(withTitle: String) -> NSMenuItem?

Returns the first menu item in the menu with a specified title.

func item(at: Int) -> NSMenuItem?

Returns the menu item at a specific location of the menu.

var numberOfItems: Int

The number of menu items in the menu, including separator items.

