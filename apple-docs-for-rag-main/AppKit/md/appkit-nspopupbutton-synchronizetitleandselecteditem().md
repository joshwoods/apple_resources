

- AppKit
- NSPopUpButton
-  synchronizeTitleAndSelectedItem() 

Instance Method

# synchronizeTitleAndSelectedItem()

Ensures that the item being displayed by the receiver agrees with the selected item.

macOS

``` source
@MainActor
func synchronizeTitleAndSelectedItem()
```

## Discussion

If there’s no selected item, this method selects the first item in the item menu and sets the receiver’s item to match. For pull-down menus, this method makes sure that the first item is being displayed (the `NSPopUpButtonCell` object must be set to use the selected menu item, which happens by default).

## See Also

### Related Documentation

var indexOfSelectedItem: Int

The index of the item that was last selected by the user.

var itemArray: [NSMenuItem]

The array of menu item objects associated with the button.

