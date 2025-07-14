

- AppKit
- NSPopUpButtonCell
-  usesItemFromMenu 

Instance Property

# usesItemFromMenu

A Boolean value that indicates if the control uses an item from the menu for its own title.

macOS

``` source
@MainActor
var usesItemFromMenu: Bool { get set }
```

## Discussion

When the value of this property is true, a pull-down menu uses the title of the first menu item, and a pop-up menu uses the title of the currently selected menu (if no menu item is selected, the pop-up button displays no item and is drawn empty). When the value is false, the menu item set with menuItem (`NSMenuItem`) is always displayed. The default value is true.

## See Also

### Accessing menu attributes

var menu: NSMenu?

The pop-up button’s associated menu.

var pullsDown: Bool

A Boolean value that indicates the behavior of the button’s menu.

var autoenablesItems: Bool

A Boolean value that indicates if the button automatically enables and disables its items every time a user event occurs.

var preferredEdge: NSRectEdge

The edge of the cell from which the menu should pop out when screen conditions are restrictive.

var altersStateOfSelectedItem: Bool

A Boolean value that indicates if the pop-up button links the state of the selected menu item to the current selection.

var arrowPosition: NSPopUpButton.ArrowPosition

The position of the arrow displayed on the button.

