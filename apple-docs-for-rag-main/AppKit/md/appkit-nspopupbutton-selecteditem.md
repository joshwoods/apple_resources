

- AppKit
- NSPopUpButton
-  selectedItem 

Instance Property

# selectedItem

The menu item that was last selected by the user.

macOS

``` source
@MainActor
var selectedItem: NSMenuItem? { get }
```

## Discussion

The last selected menu item is the one that was highlighted when the user released the mouse button. It is possible for a pull-down menu’s selected item to be its first item. If no item is selected, the value in this property is `nil`.

## See Also

### Getting the user’s selection

var titleOfSelectedItem: String?

The title of the item that was last selected by the user.

var indexOfSelectedItem: Int

The index of the item that was last selected by the user.

