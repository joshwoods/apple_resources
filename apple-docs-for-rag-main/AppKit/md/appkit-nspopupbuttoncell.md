

- AppKit
-  NSPopUpButtonCell 

Class

# NSPopUpButtonCell

The `NSPopUpButtonCell` class defines the visual appearance of pop-up buttons that display pop-up or pull-down menus. Pop-up menus present the user with a set of choices, much the way radio buttons do, but using much less space. Pull-down menus also provide a set of choices but present the information in a slightly different way, usually to provide a set of commands from which the user can choose.

macOS

``` source
@MainActor
class NSPopUpButtonCell
```

## Overview

The `NSPopUpButtonCell` class implements the user interface for the NSPopUpButton class.

Changes made to a menu (such as adding, removing, or changing the items) are not apparent while the menu is being displayed or interacted with.

Important

Setting a pop up button’s image property has no effect. The image displayed in a pop up button is taken from the selected menu item (in the case of a pop up menu) or from the first menu item (in the case of a pull-down menu).

## Topics

### Initialization

init(textCell: String, pullsDown: Bool)

Returns an `NSPopUpButtonCell` object initialized with the specified title.

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

var arrowPosition: NSPopUpButton.ArrowPosition

The position of the arrow displayed on the button.

### Adding and removing items

func addItem(withTitle: String)

Adds an item with the specified title to the end of the menu.

func addItems(withTitles: [String])

Adds multiple items to the end of the menu.

func insertItem(withTitle: String, at: Int)

Inserts an item at the specified position in the menu.

func removeItem(withTitle: String)

Removes the item with the specified title from the menu.

func removeItem(at: Int)

Removes the item at the specified index.

func removeAllItems()

Removes all items in the receiver’s item menu.

### Accessing the items

var itemArray: [NSMenuItem]

An array of NSMenuItem objects that represent the items in the menu.

var numberOfItems: Int

The number of items in the menu.

func index(of: NSMenuItem) -> Int

Returns the index of the specified menu item.

func indexOfItem(withTitle: String) -> Int

Returns the index of the item with the specified title.

func indexOfItem(withTag: Int) -> Int

Returns the index of the menu item with the specified tag.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the menu item that holds the specified represented object.

func indexOfItem(withTarget: Any?, andAction: Selector?) -> Int

Returns the index of the menu item with the specified target and action.

func item(at: Int) -> NSMenuItem?

Returns the menu item at the specified index.

func item(withTitle: String) -> NSMenuItem?

Returns the menu item with the specified title.

var lastItem: NSMenuItem?

The last item in the menu.

### Dealing with selection

func select(NSMenuItem?)

Selects the specified menu item.

func selectItem(at: Int)

Selects the item in the menu at the specified index.

func selectItem(withTag: Int) -> Bool

Selects the menu item with the specified tag.

func selectItem(withTitle: String)

Selects the item with the specified title.

func setTitle(String?)

Sets the string displayed in the receiver when the user isn’t pressing the mouse button.

var selectedItem: NSMenuItem?

The menu item last selected by the user.

var indexOfSelectedItem: Int

The index of the item last selected by the user.

func synchronizeTitleAndSelectedItem()

Synchronizes the pop-up button’s displayed item with the currently selected menu item.

### Title conveniences

func itemTitle(at: Int) -> String

Returns the title of the item at the specified index.

var itemTitles: [String]

An array of `NSString` objects containing the titles of every item in the menu.

var titleOfSelectedItem: String?

The title of the item last selected by the user.

### Handling events and action messages

func attachPopUp(withFrame: NSRect, in: NSView)

Sets up the receiver to display a menu.

func dismissPopUp()

Dismisses the pop-up button’s menu by ordering its window out.

func performClick(withFrame: NSRect, in: NSView)

Displays the receiver’s menu and track mouse events in it.

### Constants

enum ArrowPosition

These constants are defined for use with the arrowPosition property.

### Notifications

class let willPopUpNotification: NSNotification.Name

This notification is posted just before a pop-up menu is attached to its window frame.

### Initializers

init(coder: NSCoder)

## Relationships

### Inherits From

- NSMenuItemCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSMenuItemValidation
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

