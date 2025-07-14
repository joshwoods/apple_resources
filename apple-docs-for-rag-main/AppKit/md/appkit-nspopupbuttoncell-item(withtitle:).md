

- AppKit
- NSPopUpButtonCell
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

func itemTitle(at: Int) -> String

Returns the title of the item at the specified index.

### Accessing the items

var itemArray: [NSMenuItem]

An array of NSMenuItem objects that represent the items in the menu.

var numberOfItems: Int

The number of items in the menu.

func index(of: NSMenuItem) -> Int

Returns the index of the specified menu item.

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

func indexOfItem(withTag: Int) -> Int

Returns the index of the menu item with the specified tag.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the menu item that holds the specified represented object.

func indexOfItem(withTarget: Any?, andAction: Selector?) -> Int

Returns the index of the menu item with the specified target and action.

func item(at: Int) -> NSMenuItem?

Returns the menu item at the specified index.

var lastItem: NSMenuItem?

The last item in the menu.

