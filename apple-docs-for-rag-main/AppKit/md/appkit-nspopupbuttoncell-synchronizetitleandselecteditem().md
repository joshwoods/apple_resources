

- AppKit
- NSPopUpButtonCell
-  synchronizeTitleAndSelectedItem() 

Instance Method

# synchronizeTitleAndSelectedItem()

Synchronizes the pop-up button’s displayed item with the currently selected menu item.

macOS

``` source
@MainActor
func synchronizeTitleAndSelectedItem()
```

## Discussion

If no item is currently selected, this method synchronizes the pop-up buttons displayed item with the first menu item. If the pop-up button cell does not get its displayed item from a menu item, this method does nothing.

For pull-down menus, this method sets the displayed item to the title first menu item.

If the pop-up button’s menu does not contain any menu items, this method sets the pop-up button’s displayed item to `nil`, resulting in nothing being displayed in the control.

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

var selectedItem: NSMenuItem?

The menu item last selected by the user.

var indexOfSelectedItem: Int

The index of the item last selected by the user.

