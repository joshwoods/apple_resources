

- AppKit
- NSPopUpButton
-  itemTitles 

Instance Property

# itemTitles

An array of strings corresponding to the titles of the items in the menu.

macOS

``` source
@MainActor
var itemTitles: [String] { get }
```

## Discussion

This property contains an array of NSString objects, each of which contains the title of an item in the menu. The order of the titles in this array matches the order of the items in the menu. If the menu contains separator items, the array contains an empty string for each separator item.

## See Also

### Getting menu items

var menu: NSMenu?

The menu associated with the pop-up button.

var numberOfItems: Int

The number of items in the menu.

var itemArray: [NSMenuItem]

The array of menu item objects associated with the button.

func item(at: Int) -> NSMenuItem?

Returns the menu item at the specified index.

func itemTitle(at: Int) -> String

Returns the title of the item at the specified index.

func item(withTitle: String) -> NSMenuItem?

Returns the menu item with the specified title.

var lastItem: NSMenuItem?

The last item in the menu.

