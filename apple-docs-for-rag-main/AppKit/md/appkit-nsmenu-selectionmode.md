

- AppKit
- NSMenu
-  selectionMode 

Instance Property

# selectionMode

The selection mode of the menu.

macOS 14.0+

``` source
var selectionMode: NSMenu.SelectionMode { get set }
```

## Discussion

The selection mode only affects menu items that belong to the same selection group. A selection group consists of the items with the same target-action.

## See Also

### Selecting Items

var selectedItems: [NSMenuItem]

The menu items that are currently selected.

enum SelectionMode

Describes how the menu manages selection states of the menu items that belong to the same selection group.

