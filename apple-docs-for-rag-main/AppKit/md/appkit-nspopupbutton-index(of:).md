

- AppKit
- NSPopUpButton
-  index(of:) 

Instance Method

# index(of:)

Returns the index of the specified menu item.

macOS

``` source
@MainActor
func index(of item: NSMenuItem) -> Int
```

## Parameters 

`item`  

The menu item whose index you want.

## Return Value

The index of the item or `-1` if no such item was found.

## Discussion

This method invokes the method of the same name of its `NSPopUpButtonCell` object.

## See Also

### Getting the indices of menu items

func indexOfItem(withTag: Int) -> Int

Returns the index of the menu item with the specified tag.

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the menu item that holds the specified represented object.

func indexOfItem(withTarget: Any?, andAction: Selector?) -> Int

Returns the index of the menu item with the specified target and action.

