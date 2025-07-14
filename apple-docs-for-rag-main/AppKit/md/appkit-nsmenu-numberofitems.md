

- AppKit
- NSMenu
-  numberOfItems 

Instance Property

# numberOfItems

The number of menu items in the menu, including separator items.

macOS

``` source
var numberOfItems: Int { get }
```

## Discussion

This property contains a value of type `NSInteger` that indicates the number of menu items in the menu, including separator items.

## See Also

### Finding Menu Items

func item(withTag: Int) -> NSMenuItem?

Returns the first menu item in the menu with the specified tag.

func item(withTitle: String) -> NSMenuItem?

Returns the first menu item in the menu with a specified title.

func item(at: Int) -> NSMenuItem?

Returns the menu item at a specific location of the menu.

var items: [NSMenuItem]

An array containing the menu items in the menu.

