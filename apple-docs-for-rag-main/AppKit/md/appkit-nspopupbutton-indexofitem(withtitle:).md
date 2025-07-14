

- AppKit
- NSPopUpButton
-  indexOfItem(withTitle:) 

Instance Method

# indexOfItem(withTitle:)

Returns the index of the item with the specified title.

macOS

``` source
@MainActor
func indexOfItem(withTitle title: String) -> Int
```

## Parameters 

`title`  

The title of the item you want.

## Return Value

The index of the item or `-1` if no item with the specified title was found.

## See Also

### Getting the indices of menu items

func index(of: NSMenuItem) -> Int

Returns the index of the specified menu item.

func indexOfItem(withTag: Int) -> Int

Returns the index of the menu item with the specified tag.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the menu item that holds the specified represented object.

func indexOfItem(withTarget: Any?, andAction: Selector?) -> Int

Returns the index of the menu item with the specified target and action.

