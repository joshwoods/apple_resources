

- AppKit
- NSPopUpButton
-  item(withTitle:) 

Instance Method

# item(withTitle:)

Returns the menu item with the specified title.

macOS

``` source
@MainActor
func item(withTitle title: String) -> NSMenuItem?
```

## Parameters 

`title`  

The title of the menu item you want.

## Return Value

The menu item, or `nil` if no item with the specified title exists in the menu.

## See Also

### Related Documentation

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

func addItem(withTitle: String)

Adds an item with the specified title to the end of the menu.

func selectItem(withTitle: String)

Selects the item with the specified title.

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

var itemTitles: [String]

An array of strings corresponding to the titles of the items in the menu.

var lastItem: NSMenuItem?

The last item in the menu.

