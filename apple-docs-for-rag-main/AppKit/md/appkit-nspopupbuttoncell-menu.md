

- AppKit
- NSPopUpButtonCell
-  menu 

Instance Property

# menu

The pop-up button’s associated menu.

macOS

``` source
@MainActor
var menu: NSMenu? { get set }
```

## See Also

### Accessing menu attributes

var pullsDown: Bool

A Boolean value that indicates the behavior of the button’s menu.

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

