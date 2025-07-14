

- AppKit
- NSPopUpButton
-  indexOfItem(withRepresentedObject:) 

Instance Method

# indexOfItem(withRepresentedObject:)

Returns the index of the menu item that holds the specified represented object.

macOS

``` source
@MainActor
func indexOfItem(withRepresentedObject obj: Any?) -> Int
```

## Parameters 

`obj`  

The represented object associated with a menu item.

## Return Value

The index of the menu item that owns the specified object, or `-1` if no such menu item was found.

## Discussion

Represented objects bear some direct relation to the title or image of a menu item; for example, an item entitled “100” might have an `NSNumber` object encapsulating that value as its represented object. This method invokes the method of the same name of its `NSPopUpButtonCell` object.

## See Also

### Getting the indices of menu items

func index(of: NSMenuItem) -> Int

Returns the index of the specified menu item.

func indexOfItem(withTag: Int) -> Int

Returns the index of the menu item with the specified tag.

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

func indexOfItem(withTarget: Any?, andAction: Selector?) -> Int

Returns the index of the menu item with the specified target and action.

