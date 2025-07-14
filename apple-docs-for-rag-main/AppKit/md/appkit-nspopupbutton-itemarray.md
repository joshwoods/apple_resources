

- AppKit
- NSPopUpButton
-  itemArray 

Instance Property

# itemArray

The array of menu item objects associated with the button.

macOS

``` source
@MainActor
var itemArray: [NSMenuItem] { get }
```

## Discussion

This property contains an array of NSMenuItem objects representing the items in the menu. Usually, you access menu items using the methods and properties of this class rather than accessing the items directly.

## See Also

### Related Documentation

func insertItem(withTitle: String, at: Int)

Inserts an item at the specified position in the menu.

func removeItem(at: Int)

Removes the item at the specified index.

### Getting menu items

var menu: NSMenu?

The menu associated with the pop-up button.

var numberOfItems: Int

The number of items in the menu.

func item(at: Int) -> NSMenuItem?

Returns the menu item at the specified index.

func itemTitle(at: Int) -> String

Returns the title of the item at the specified index.

var itemTitles: [String]

An array of strings corresponding to the titles of the items in the menu.

func item(withTitle: String) -> NSMenuItem?

Returns the menu item with the specified title.

var lastItem: NSMenuItem?

The last item in the menu.

