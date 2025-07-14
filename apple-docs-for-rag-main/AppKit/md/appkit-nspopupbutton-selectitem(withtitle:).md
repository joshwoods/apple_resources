

- AppKit
- NSPopUpButton
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

## See Also

### Related Documentation

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

func addItem(withTitle: String)

Adds an item with the specified title to the end of the menu.

func setTitle(String)

Sets the string displayed in the receiver when the user isn’t pressing the mouse button.

### Setting the current selection

func select(NSMenuItem?)

Selects the specified menu item.

func selectItem(at: Int)

Selects the item in the menu at the specified index.

func selectItem(withTag: Int) -> Bool

Selects the menu item with the specified tag.

