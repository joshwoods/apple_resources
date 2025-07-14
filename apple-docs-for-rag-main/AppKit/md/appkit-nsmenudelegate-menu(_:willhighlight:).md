

- AppKit
- NSMenuDelegate
-  menu(\_:willHighlight:) 

Instance Method

# menu(\_:willHighlight:)

Invoked to indicate that a menu is about to highlight a given item.

macOS 10.5+

``` source
@MainActor
optional func menu(
    _ menu: NSMenu,
    willHighlight item: NSMenuItem?
)
```

## Parameters 

`menu`  

The menu object about to highlight an item.

`item`  

The item about to be highlighted.

## Discussion

Only one item per menu can be highlighted at a time. If `item` is `nil`, it means that all items in the menu are about to be unhighlighted.

## See Also

### Related Documentation

var highlightedItem: NSMenuItem?

Indicates the currently highlighted item in the menu.

