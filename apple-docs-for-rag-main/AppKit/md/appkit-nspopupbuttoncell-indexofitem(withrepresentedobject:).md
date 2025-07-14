

- AppKit
- NSPopUpButtonCell
-  indexOfItem(withRepresentedObject:) 

Instance Method

# indexOfItem(withRepresentedObject:)

Returns the index of the menu item that holds the specified represented object.

macOS

``` source
@MainActor
func indexOfItem(withRepresentedObject obj: Any?) -> Int
```

## Parameters 

`obj`  

The represented object associated with a menu item.

## Return Value

The index of the menu item that owns the specified object, or `-1` if no such menu item was found.

## See Also

### Related Documentation

var indexOfSelectedItem: Int

The index of the item last selected by the user.

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

func indexOfItem(withTarget: Any?, andAction: Selector?) -> Int

Returns the index of the menu item with the specified target and action.

func item(at: Int) -> NSMenuItem?

Returns the menu item at the specified index.

func item(withTitle: String) -> NSMenuItem?

Returns the menu item with the specified title.

var lastItem: NSMenuItem?

The last item in the menu.

