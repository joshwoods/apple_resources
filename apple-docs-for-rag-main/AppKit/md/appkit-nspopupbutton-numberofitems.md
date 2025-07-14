

- AppKit
- NSPopUpButton
-  numberOfItems 

Instance Property

# numberOfItems

The number of items in the menu.

macOS

``` source
@MainActor
var numberOfItems: Int { get }
```

## See Also

### Getting menu items

var menu: NSMenu?

The menu associated with the pop-up button.

var itemArray: [NSMenuItem]

The array of menu item objects associated with the button.

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

