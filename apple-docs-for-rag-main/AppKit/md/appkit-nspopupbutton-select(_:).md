

- AppKit
- NSPopUpButton
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

## See Also

### Setting the current selection

func selectItem(at: Int)

Selects the item in the menu at the specified index.

func selectItem(withTag: Int) -> Bool

Selects the menu item with the specified tag.

func selectItem(withTitle: String)

Selects the item with the specified title.

