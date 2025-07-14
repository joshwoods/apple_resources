

- AppKit
- NSMenu
-  item(at:) 

Instance Method

# item(at:)

Returns the menu item at a specific location of the menu.

macOS

``` source
func item(at index: Int) -> NSMenuItem?
```

## Parameters 

`index`  

An integer index locating a menu item in a menu.

## Return Value

The found menu item (an object conforming to the NSMenuItem protocol) or `nil` if the object couldn’t be found.

## Discussion

This method raises an exception if `index` is out of bounds.

## See Also

### Related Documentation

func index(of: NSMenuItem) -> Int

Returns the index identifying the location of a specified menu item in the menu.

### Finding Menu Items

func item(withTag: Int) -> NSMenuItem?

Returns the first menu item in the menu with the specified tag.

func item(withTitle: String) -> NSMenuItem?

Returns the first menu item in the menu with a specified title.

var numberOfItems: Int

The number of menu items in the menu, including separator items.

var items: [NSMenuItem]

An array containing the menu items in the menu.

