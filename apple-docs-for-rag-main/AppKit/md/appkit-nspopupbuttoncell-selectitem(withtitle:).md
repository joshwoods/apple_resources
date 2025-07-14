

- AppKit
- NSPopUpButtonCell
-  selectItem(withTitle:) 

Instance Method

# selectItem(withTitle:)

Selects the item with the specified title.

macOS

``` source
@MainActor
func selectItem(withTitle title: String)
```

## Parameters 

`title`  

The title of the item to select. If you specify an empty string, or a string that does not match the title of a menu item, this method deselects the currently selected item.

## Discussion

By default, selecting or deselecting a menu item changes its state. To disassociate the current selection from the state of menu items, set the altersStateOfSelectedItem property to false.

## See Also

### Related Documentation

var altersStateOfSelectedItem: Bool

A Boolean value that indicates if the pop-up button links the state of the selected menu item to the current selection.

### Dealing with selection

func select(NSMenuItem?)

Selects the specified menu item.

func selectItem(at: Int)

Selects the item in the menu at the specified index.

func selectItem(withTag: Int) -> Bool

Selects the menu item with the specified tag.

func setTitle(String?)

Sets the string displayed in the receiver when the user isn’t pressing the mouse button.

var selectedItem: NSMenuItem?

The menu item last selected by the user.

var indexOfSelectedItem: Int

The index of the item last selected by the user.

func synchronizeTitleAndSelectedItem()

Synchronizes the pop-up button’s displayed item with the currently selected menu item.

