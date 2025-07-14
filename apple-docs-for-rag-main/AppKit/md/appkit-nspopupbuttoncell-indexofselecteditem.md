

- AppKit
- NSPopUpButtonCell
-  indexOfSelectedItem 

Instance Property

# indexOfSelectedItem

The index of the item last selected by the user.

macOS

``` source
@MainActor
var indexOfSelectedItem: Int { get }
```

## Discussion

The value of this property is the index of the selected item, or `-1` if no item is selected.

## See Also

### Related Documentation

func indexOfItem(withTag: Int) -> Int

Returns the index of the menu item with the specified tag.

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

func index(of: NSMenuItem) -> Int

Returns the index of the specified menu item.

func indexOfItem(withTarget: Any?, andAction: Selector?) -> Int

Returns the index of the menu item with the specified target and action.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the menu item that holds the specified represented object.

### Dealing with selection

func select(NSMenuItem?)

Selects the specified menu item.

func selectItem(at: Int)

Selects the item in the menu at the specified index.

func selectItem(withTag: Int) -> Bool

Selects the menu item with the specified tag.

func selectItem(withTitle: String)

Selects the item with the specified title.

func setTitle(String?)

Sets the string displayed in the receiver when the user isn’t pressing the mouse button.

var selectedItem: NSMenuItem?

The menu item last selected by the user.

func synchronizeTitleAndSelectedItem()

Synchronizes the pop-up button’s displayed item with the currently selected menu item.

