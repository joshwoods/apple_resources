

- AppKit
- NSPopUpButtonCell
-  selectItem(withTag:) 

Instance Method

# selectItem(withTag:)

Selects the menu item with the specified tag.

macOS

``` source
@MainActor
func selectItem(withTag tag: Int) -> Bool
```

## Parameters 

`tag`  

The tag of the item you want to select.

## Return Value

true if the item was successfully selected; otherwise, false.

## Discussion

If no item with the specified tag is found, this method returns false and leaves the menu state unchanged.

You typically assign tags to menu items from Interface Builder, but you can also assign them programmatically using the setTag: method of NSMenuItem.

## See Also

### Dealing with selection

func select(NSMenuItem?)

Selects the specified menu item.

func selectItem(at: Int)

Selects the item in the menu at the specified index.

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

