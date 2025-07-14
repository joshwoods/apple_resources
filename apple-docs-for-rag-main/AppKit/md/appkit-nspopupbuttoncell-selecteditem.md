

- AppKit
- NSPopUpButtonCell
-  selectedItem 

Instance Property

# selectedItem

The menu item last selected by the user.

macOS

``` source
@MainActor
var selectedItem: NSMenuItem? { get }
```

## Discussion

The value of this property is the menu item that is currently selected, or `nil` if no item is selected. The last selected menu item is the one that was highlighted when the user released the mouse button. It is possible for a pull-down menu’s selected item to be its first item.

## See Also

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

var indexOfSelectedItem: Int

The index of the item last selected by the user.

func synchronizeTitleAndSelectedItem()

Synchronizes the pop-up button’s displayed item with the currently selected menu item.

