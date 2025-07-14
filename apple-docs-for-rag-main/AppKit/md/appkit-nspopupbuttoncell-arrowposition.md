

- AppKit
- NSPopUpButtonCell
-  arrowPosition 

Instance Property

# arrowPosition

The position of the arrow displayed on the button.

macOS

``` source
@MainActor
var arrowPosition: NSPopUpButton.ArrowPosition { get set }
```

## Discussion

When the value of this property is NSPopUpButton.ArrowPosition.noArrow, the control displays no arrow. NSPopUpButton.ArrowPosition.arrowAtCenter displays the arrow centered horizontally within the cell and NSPopUpButton.ArrowPosition.arrowAtBottom displays the arrow at the edge of the cell. This property is used with preferredEdge to determine the exact location and orientation of the arrow.

This property applies to only bezel style and borderless pop-up buttons.

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

var usesItemFromMenu: Bool

A Boolean value that indicates if the control uses an item from the menu for its own title.

var altersStateOfSelectedItem: Bool

A Boolean value that indicates if the pop-up button links the state of the selected menu item to the current selection.

