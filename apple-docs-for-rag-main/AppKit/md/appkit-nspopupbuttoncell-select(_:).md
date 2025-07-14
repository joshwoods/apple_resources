

- AppKit
- NSPopUpButtonCell
-  select(\_:) 

Instance Method

# select(\_:)

Selects the specified menu item.

macOS

``` source
@MainActor
func select(_ item: NSMenuItem?)
```

## Parameters 

`item`  

The menu item to select, or `nil` if you want to deselect all menu items.

## Discussion

By default, selecting or deselecting a menu item from a pop-up menu changes its state. Selecting a menu item from a pull-down menu does not automatically alter the state of the item. To disassociate the current selection from the state of menu items, set the altersStateOfSelectedItem property to false.

## See Also

### Related Documentation

var altersStateOfSelectedItem: Bool

A Boolean value that indicates if the pop-up button links the state of the selected menu item to the current selection.

### Dealing with selection

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

var indexOfSelectedItem: Int

The index of the item last selected by the user.

func synchronizeTitleAndSelectedItem()

Synchronizes the pop-up button’s displayed item with the currently selected menu item.

