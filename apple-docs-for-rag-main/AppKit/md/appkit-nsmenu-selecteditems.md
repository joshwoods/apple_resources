

- AppKit
- NSMenu
-  selectedItems 

Instance Property

# selectedItems

The menu items that are currently selected.

macOS 14.0+

``` source
var selectedItems: [NSMenuItem] { get set }
```

## Discussion

An item selects when its state is on. If the tracking mode is NSMenu.SelectionMode.selectOne or NSMenu.SelectionMode.selectAny, the property only selects or returns menu items whose show-target action is `nil`.

## See Also

### Selecting Items

var selectionMode: NSMenu.SelectionMode

The selection mode of the menu.

enum SelectionMode

Describes how the menu manages selection states of the menu items that belong to the same selection group.

