

- AppKit
-  NSMenu 

Class

# NSMenu

An object that manages an app’s menus.

macOS

``` source
class NSMenu
```

## Topics

### Managing the Menu Bar

class func menuBarVisible() -> Bool

Returns a Boolean value that indicates whether the menu bar is visible.

class func setMenuBarVisible(Bool)

Sets whether the menu bar is visible and selectable by the user.

var menuBarHeight: CGFloat

The menu bar height for the main menu in pixels.

### Creating an NSMenu Object

init(title: String)

Initializes and returns a menu having the specified title and with autoenabling of menu items turned on.

init(coder: NSCoder)

### Adding and Removing Menu Items

func insertItem(NSMenuItem, at: Int)

Inserts a menu item into the menu at a specific location.

func insertItem(withTitle: String, action: Selector?, keyEquivalent: String, at: Int) -> NSMenuItem

Creates and adds a menu item at a specified location in the menu.

func addItem(NSMenuItem)

Adds a menu item to the end of the menu.

func addItem(withTitle: String, action: Selector?, keyEquivalent: String) -> NSMenuItem

Creates a new menu item and adds it to the end of the menu.

func removeItem(NSMenuItem)

Removes a menu item from the menu.

func removeItem(at: Int)

Removes the menu item at a specified location in the menu.

func itemChanged(NSMenuItem)

Invoked when a menu item is modified visually (for example, its title changes).

func removeAllItems()

Removes all the menu items in the menu.

### Finding Menu Items

func item(withTag: Int) -> NSMenuItem?

Returns the first menu item in the menu with the specified tag.

func item(withTitle: String) -> NSMenuItem?

Returns the first menu item in the menu with a specified title.

func item(at: Int) -> NSMenuItem?

Returns the menu item at a specific location of the menu.

var numberOfItems: Int

The number of menu items in the menu, including separator items.

var items: [NSMenuItem]

An array containing the menu items in the menu.

### Finding Indices of Menu Items

func index(of: NSMenuItem) -> Int

Returns the index identifying the location of a specified menu item in the menu.

func indexOfItem(withTitle: String) -> Int

Returns the index of the first menu item in the menu that has a specified title.

func indexOfItem(withTag: Int) -> Int

Returns the index of the first menu item in the menu identified by a tag.

func indexOfItem(withTarget: Any?, andAction: Selector?) -> Int

Returns the index of the first menu item in the menu that has a specified action and target.

func indexOfItem(withRepresentedObject: Any?) -> Int

Returns the index of the first menu item in the menu that has a given represented object.

func indexOfItem(withSubmenu: NSMenu?) -> Int

Returns the index of the menu item in the menu with the given submenu.

### Managing Submenus

func setSubmenu(NSMenu?, for: NSMenuItem)

Assigns a menu to be a submenu of the menu controlled by a given menu item.

func submenuAction(Any?)

The action method assigned to menu items that open submenus.

var supermenu: NSMenu?

The parent menu that contains the menu as a submenu.

var isTornOff: Bool

Indicates whether the menu is offscreen or attached to another menu (or if it’s the main menu).

Deprecated

### Enabling and Disabling Menu Items

var autoenablesItems: Bool

Indicates whether the menu automatically enables and disables its menu items.

func update()

Enables or disables the menu items of the menu based on the NSMenuValidation informal protocol and sizes the menu to fit its current menu items if necessary.

### Getting and Setting the Menu Font

var font: NSFont!

The font of the menu and its submenus.

### Handling Keyboard Equivalents

func performKeyEquivalent(with: NSEvent) -> Bool

Performs the action for the menu item that corresponds to the given key equivalent.

### Simulating Mouse Clicks

func performActionForItem(at: Int)

Causes the application to send the action message of a specified menu item to its target.

### Managing the Title

var title: String

The title of the menu.

### Selecting Items

var selectedItems: [NSMenuItem]

The menu items that are currently selected.

var selectionMode: NSMenu.SelectionMode

The selection mode of the menu.

enum SelectionMode

Describes how the menu manages selection states of the menu items that belong to the same selection group.

### Configuring Menu Size

var minimumWidth: CGFloat

The minimum width of the menu in screen coordinates.

var size: NSSize

The size of the menu in screen coordinates

### Getting Menu Properties

var propertiesToUpdate: NSMenu.Properties

The available properties for the menu.

### Managing Presentation Styles

var presentationStyle: NSMenu.PresentationStyle

The presentation style of the menu.

enum PresentationStyle

Specifies the style of a menu.

### Working with Palettes

static func palette(colors: [NSColor], titles: [String], template: NSImage?, onSelectionChange: ((NSMenu) -> Void)?) -> NSMenu

Creates a palette style menu displaying user-selectable color tags that tint using the specified array of colors.

### Managing Menu Change Notifications

var menuChangedMessagesEnabled: Bool

Indicates whether messages are sent to the application’s windows each time the menu changes.

Deprecated

### Displaying Contextual Menus

var allowsContextMenuPlugIns: Bool

Indicates whether the pop-up menu allows appending of contextual menu plug-in items.

### Displaying Context-Sensitive Help

class func popUpContextMenu(NSMenu, with: NSEvent, for: NSView)

Displays a contextual menu over a view for an event.

class func popUpContextMenu(NSMenu, with: NSEvent, for: NSView, with: NSFont?)

Displays a contextual menu over a view for an event using a specified font.

func helpRequested(with: NSEvent)

Overridden by subclasses to implement specialized context-sensitive help behavior.

Deprecated

func popUp(positioning: NSMenuItem?, at: NSPoint, in: NSView?) -> Bool

Pops up the menu at the specified location.

### Managing Display of the State Column

var showsStateColumn: Bool

Indicates whether the menu displays the state column.

### Controlling Allocation Zones

class func menuZone() -> NSZone!

Returns the zone from which `NSMenu` objects should be allocated.

Deprecated

### Handling Highlighting

var highlightedItem: NSMenuItem?

Indicates the currently highlighted item in the menu.

### Managing the User Interface

var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection

Configures the layout direction of menu items in the menu.

### Managing the Delegate

var delegate: (any NSMenuDelegate)?

The delegate of the menu.

### Handling Tracking

func cancelTracking()

Dismisses the menu and ends all menu tracking.

func cancelTrackingWithoutAnimation()

Dismisses the menu and ends all menu tracking without displaying the associated animation.

### Constants

struct Properties

These constants are used as a bitmask for specifying a set of menu or menu item properties, and are contained by the propertiesToUpdate property.

### Notifications

class let didAddItemNotification: NSNotification.Name

Posted after a menu item is added to the menu.

class let didChangeItemNotification: NSNotification.Name

Posted after a menu item in the menu changes appearance.

class let didBeginTrackingNotification: NSNotification.Name

Posted when menu tracking begins.

class let didEndTrackingNotification: NSNotification.Name

Posted when menu tracking ends, even if no action is sent.

class let didRemoveItemNotification: NSNotification.Name

Posted after a menu item is removed from the menu.

class let didSendActionNotification: NSNotification.Name

Posted just after the application dispatches a menu item’s action method to the menu item’s target.

class let willSendActionNotification: NSNotification.Name

Posted just before the application dispatches a menu item’s action method to the menu item’s target.

### Instance Properties

var automaticallyInsertsWritingToolsItems: Bool

### Instance Methods

func isJavaMenu() -> Bool

func setJavaMenuDelegate((any JRSMenuDelegate)!)

### Type Methods

class func javaMenu(withTitle: String!) -> NSMenu!

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAppearanceCustomization
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification

## See Also

### Menus

class NSMenuItem

A command item in an app menu.

class NSMenuItemBadge

A control that provides additional quantitative information specific to a menu item, such as the number of available updates.

protocol NSMenuDelegate

The optional methods implemented by delegates of NSMenu objects to manage menu display and handle some events.

