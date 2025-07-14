

- AppKit
- NSPopUpButton
-  itemTitle(at:) 

Instance Method

# itemTitle(at:)

Returns the title of the item at the specified index.

macOS

``` source
@MainActor
func itemTitle(at index: Int) -> String
```

## Parameters 

`index`  

The index of the item you want.

## Return Value

The title of the item, or an empty string if no item exists at the specified index.

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

var itemTitles: [String]

An array of strings corresponding to the titles of the items in the menu.

func item(withTitle: String) -> NSMenuItem?

Returns the menu item with the specified title.

var lastItem: NSMenuItem?

The last item in the menu.

