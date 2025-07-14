

- AppKit
- NSPopUpButton
-  selectItem(at:) 

Instance Method

# selectItem(at:)

Selects the item in the menu at the specified index.

macOS

``` source
@MainActor
func selectItem(at index: Int)
```

## Parameters 

`index`  

The index of the item you want to select, or `-1` you want to deselect all menu items.

## See Also

### Related Documentation

var indexOfSelectedItem: Int

The index of the item that was last selected by the user.

### Setting the current selection

func select(NSMenuItem?)

Selects the specified menu item.

func selectItem(withTag: Int) -> Bool

Selects the menu item with the specified tag.

func selectItem(withTitle: String)

Selects the item with the specified title.

