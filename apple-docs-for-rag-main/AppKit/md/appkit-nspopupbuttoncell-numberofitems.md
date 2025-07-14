

- AppKit
- NSPopUpButtonCell
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

### Related Documentation

var count: Int

The number of objects in the array.

### Accessing the items

var itemArray: [NSMenuItem]

An array of NSMenuItem objects that represent the items in the menu.

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

func item(withTitle: String) -> NSMenuItem?

Returns the menu item with the specified title.

var lastItem: NSMenuItem?

The last item in the menu.

