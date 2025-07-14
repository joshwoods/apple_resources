

- AppKit
- NSPopUpButton
-  indexOfItem(withTag:) 

Instance Method

# indexOfItem(withTag:)

Returns the index of the menu item with the specified tag.

macOS

``` source
@MainActor
func indexOfItem(withTag tag: Int) -> Int
```

## Parameters 

`tag`  

The tag of the menu item you want.

## Return Value

The index of the item or `-1` if no item with the specified tag was found.

## Discussion

This method invokes the method of the same name of its `NSPopUpButtonCell` object.

## See Also

### Getting the indices of menu items

func index(of: NSMenuItem) -> Int

Returns the index of the specified menu item.

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the menu item that holds the specified represented object.

func indexOfItem(withTarget: Any?, andAction: Selector?) -> Int

Returns the index of the menu item with the specified target and action.

