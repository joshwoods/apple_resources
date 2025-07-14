

- AppKit
- NSPopUpButtonCell
-  pullsDown 

Instance Property

# pullsDown

A Boolean value that indicates the behavior of the button’s menu.

macOS

``` source
@MainActor
var pullsDown: Bool { get set }
```

## Discussion

When the value of this property is true, the menu behaves like a pull-down menu; when the value is false, it behaves like a pop-up menu. If you use this property to change the menu type from a pop-up menu to a pull-down menu, and the cell alters the state of its selected items, the state of the currently selected item is set to NSOffState before the menu type is changed.

## See Also

### Related Documentation

func synchronizeTitleAndSelectedItem()

Synchronizes the pop-up button’s displayed item with the currently selected menu item.

### Accessing menu attributes

var menu: NSMenu?

The pop-up button’s associated menu.

var autoenablesItems: Bool

A Boolean value that indicates if the button automatically enables and disables its items every time a user event occurs.

var preferredEdge: NSRectEdge

The edge of the cell from which the menu should pop out when screen conditions are restrictive.

var usesItemFromMenu: Bool

A Boolean value that indicates if the control uses an item from the menu for its own title.

var altersStateOfSelectedItem: Bool

A Boolean value that indicates if the pop-up button links the state of the selected menu item to the current selection.

var arrowPosition: NSPopUpButton.ArrowPosition

The position of the arrow displayed on the button.

