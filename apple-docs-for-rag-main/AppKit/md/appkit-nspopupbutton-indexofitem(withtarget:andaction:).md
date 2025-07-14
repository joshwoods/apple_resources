

- AppKit
- NSPopUpButton
-  indexOfItem(withTarget:andAction:) 

Instance Method

# indexOfItem(withTarget:andAction:)

Returns the index of the menu item with the specified target and action.

macOS

``` source
@MainActor
func indexOfItem(
    withTarget target: Any?,
    andAction actionSelector: Selector?
) -> Int
```

## Parameters 

`target`  

The target object associated with the menu item.

`actionSelector`  

The action method associated with the menu item.

## Return Value

The index of the menu item, or `-1` if no menu item contains the specified target and action.

## Discussion

If you specify `NULL` for the `actionSelector` parameter, the index of the first menu item with the specified target is returned. This method invokes the method of the same name of its `NSPopUpButtonCell` object.

## See Also

### Getting the indices of menu items

func index(of: NSMenuItem) -> Int

Returns the index of the specified menu item.

func indexOfItem(withTag: Int) -> Int

Returns the index of the menu item with the specified tag.

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the menu item that holds the specified represented object.

