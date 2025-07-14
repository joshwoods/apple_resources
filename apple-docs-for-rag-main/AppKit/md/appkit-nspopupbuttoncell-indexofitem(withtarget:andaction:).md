

- AppKit
- NSPopUpButtonCell
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

If you specify `NULL` for the `actionSelector` parameter, the index of the first menu item with the specified target is returned.

The `NSPopUpButtonCell` class assigns a default action and target to each menu item, but you can change these values using the setAction: and setTarget: methods of NSMenuItem.

## See Also

### Related Documentation

var indexOfSelectedItem: Int

The index of the item last selected by the user.

### Accessing the items

var itemArray: [NSMenuItem]

An array of NSMenuItem objects that represent the items in the menu.

var numberOfItems: Int

The number of items in the menu.

func index(of: NSMenuItem) -> Int

Returns the index of the specified menu item.

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

func indexOfItem(withTag: Int) -> Int

Returns the index of the menu item with the specified tag.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the menu item that holds the specified represented object.

func item(at: Int) -> NSMenuItem?

Returns the menu item at the specified index.

func item(withTitle: String) -> NSMenuItem?

Returns the menu item with the specified title.

var lastItem: NSMenuItem?

The last item in the menu.

