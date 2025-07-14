

- AppKit
-  NSMenuDelegate 

Protocol

# NSMenuDelegate

The optional methods implemented by delegates of NSMenu objects to manage menu display and handle some events.

macOS

``` source
protocol NSMenuDelegate : NSObjectProtocol
```

## Topics

### Handling Keyboard Equivalents

func menuHasKeyEquivalent(NSMenu, for: NSEvent, target: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, action: UnsafeMutablePointer&lt;Selector?>) -> Bool

Invoked to allow the delegate to return the target and action for a key-down event.

### Updating Menu Layout

func menu(NSMenu, update: NSMenuItem, at: Int, shouldCancel: Bool) -> Bool

Invoked to let the delegate update a menu item before it is displayed.

func confinementRect(for: NSMenu, on: NSScreen?) -> NSRect

Invoked to allow the delegate to specify a display location for the menu.

### Handling Highlighting

func menu(NSMenu, willHighlight: NSMenuItem?)

Invoked to indicate that a menu is about to highlight a given item.

### Handling Open and Close Events

func menuWillOpen(NSMenu)

Invoked when a menu is about to open.

func menuDidClose(NSMenu)

Invoked after a menu closed.

### Handling Tracking

func numberOfItems(in: NSMenu) -> Int

Invoked when a menu is about to be displayed at the start of a tracking session so the delegate can specify the number of items in the menu.

func menuNeedsUpdate(NSMenu)

Invoked when a menu is about to be displayed at the start of a tracking session.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Menus

class NSMenu

An object that manages an app’s menus.

class NSMenuItem

A command item in an app menu.

class NSMenuItemBadge

A control that provides additional quantitative information specific to a menu item, such as the number of available updates.

