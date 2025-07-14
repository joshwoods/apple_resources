

- AppKit
- NSPopUpButtonCell
-  setTitle(\_:) 

Instance Method

# setTitle(\_:)

Sets the string displayed in the receiver when the user isn’t pressing the mouse button.

macOS

``` source
@MainActor
func setTitle(_ string: String?)
```

## Parameters 

`string`  

The string to display.

## Discussion

For pull-down menus that get their titles from a menu item, this method simply sets the pop-up button cell’s menu item to the first item in the menu. For pop-up menus, if a menu item whose title matches `aString` exists, this method makes that menu item the current selection; otherwise, it creates a new menu item with the title `aString`, adds it to the pop-up menu, and selects it.

## See Also

### Related Documentation

init(textCell: String, pullsDown: Bool)

Returns an `NSPopUpButtonCell` object initialized with the specified title.

### Dealing with selection

func select(NSMenuItem?)

Selects the specified menu item.

func selectItem(at: Int)

Selects the item in the menu at the specified index.

func selectItem(withTag: Int) -> Bool

Selects the menu item with the specified tag.

func selectItem(withTitle: String)

Selects the item with the specified title.

var selectedItem: NSMenuItem?

The menu item last selected by the user.

var indexOfSelectedItem: Int

The index of the item last selected by the user.

func synchronizeTitleAndSelectedItem()

Synchronizes the pop-up button’s displayed item with the currently selected menu item.

