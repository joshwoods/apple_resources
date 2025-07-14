

- AppKit
- NSPopUpButton
-  item(at:) 

Instance Method

# item(at:)

Returns the menu item at the specified index.

macOS

``` source
@MainActor
func item(at index: Int) -> NSMenuItem?
```

## Parameters 

`index`  

The index of the item you want.

## Return Value

The menu item, or `nil` if no item exists at the specified index.

## See Also

### Getting menu items

var menu: NSMenu?

The menu associated with the pop-up button.

var numberOfItems: Int

The number of items in the menu.

var itemArray: [NSMenuItem]

The array of menu item objects associated with the button.

func itemTitle(at: Int) -> String

Returns the title of the item at the specified index.

var itemTitles: [String]

An array of strings corresponding to the titles of the items in the menu.

func item(withTitle: String) -> NSMenuItem?

Returns the menu item with the specified title.

var lastItem: NSMenuItem?

The last item in the menu.

