

- AppKit
- NSPopUpButtonCell
-  altersStateOfSelectedItem 

Instance Property

# altersStateOfSelectedItem

A Boolean value that indicates if the pop-up button links the state of the selected menu item to the current selection.

macOS

``` source
@MainActor
var altersStateOfSelectedItem: Bool { get set }
```

## Discussion

When the value of this property is true (which is the default value), the state of the selected item is set to NSOnState. When the value of this property is false, the items in the menu are left alone. When you change the value of this property, the state of the currently selected item is updated appropriately.

Note that this property affects only pop-up buttons (it is ignored for pull-down menus).

## See Also

### Related Documentation

func selectItem(at: Int)

Selects the item in the menu at the specified index.

func select(NSMenuItem?)

Selects the specified menu item.

var selectedItem: NSMenuItem?

The menu item last selected by the user.

func selectItem(withTitle: String)

Selects the item with the specified title.

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

var arrowPosition: NSPopUpButton.ArrowPosition

The position of the arrow displayed on the button.

