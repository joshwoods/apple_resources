

- AppKit
- NSPopUpButtonCell
-  index(of:) 

Instance Method

# index(of:)

Returns the index of the specified menu item.

macOS

``` source
@MainActor
func index(of item: NSMenuItem) -> Int
```

## Parameters 

`item`  

The menu item whose index you want.

## Return Value

The index of the item or `-1` if no such item was found.

## See Also

### Related Documentation

var indexOfSelectedItem: Int

The index of the item last selected by the user.

### Accessing the items

var itemArray: [NSMenuItem]

An array of NSMenuItem objects that represent the items in the menu.

var numberOfItems: Int

The number of items in the menu.

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

func item(withTitle: String) -> NSMenuItem?

Returns the menu item with the specified title.

var lastItem: NSMenuItem?

The last item in the menu.

