

- AppKit
- NSPopUpButtonCell
-  autoenablesItems 

Instance Property

# autoenablesItems

A Boolean value that indicates if the button automatically enables and disables its items every time a user event occurs.

macOS

``` source
@MainActor
var autoenablesItems: Bool { get set }
```

## Discussion

When the value of this property is true, the button automatically enables and disables items. The default value is true. For more information about enabling and disabling menu items, see NSMenuValidation.

## See Also

### Accessing menu attributes

var menu: NSMenu?

The pop-up button’s associated menu.

var pullsDown: Bool

A Boolean value that indicates the behavior of the button’s menu.

var preferredEdge: NSRectEdge

The edge of the cell from which the menu should pop out when screen conditions are restrictive.

var usesItemFromMenu: Bool

A Boolean value that indicates if the control uses an item from the menu for its own title.

var altersStateOfSelectedItem: Bool

A Boolean value that indicates if the pop-up button links the state of the selected menu item to the current selection.

var arrowPosition: NSPopUpButton.ArrowPosition

The position of the arrow displayed on the button.

