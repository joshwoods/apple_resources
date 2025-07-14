

- AppKit
- NSPopUpButton
-  indexOfSelectedItem 

Instance Property

# indexOfSelectedItem

The index of the item that was last selected by the user.

macOS

``` source
@MainActor
var indexOfSelectedItem: Int { get }
```

## Discussion

If no item is selected, the value in this property is `-1`.

## See Also

### Getting the user’s selection

var selectedItem: NSMenuItem?

The menu item that was last selected by the user.

var titleOfSelectedItem: String?

The title of the item that was last selected by the user.

