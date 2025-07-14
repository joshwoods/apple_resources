

- AppKit
- NSPopUpButton
-  titleOfSelectedItem 

Instance Property

# titleOfSelectedItem

The title of the item that was last selected by the user.

macOS

``` source
@MainActor
var titleOfSelectedItem: String? { get }
```

## Discussion

If no item is selected, the value in this property is `nil`.

## See Also

### Getting the user’s selection

var selectedItem: NSMenuItem?

The menu item that was last selected by the user.

var indexOfSelectedItem: Int

The index of the item that was last selected by the user.

