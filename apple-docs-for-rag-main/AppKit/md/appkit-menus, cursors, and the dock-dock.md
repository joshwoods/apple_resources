

- AppKit
-  Menus, Cursors, and the Dock 

API Collection

# Menus, Cursors, and the Dock

Implement menus and cursors to facilitate interactions with your app, and use your app’s Dock tile to convey updated information.

## Topics

### Menus

class NSMenu

An object that manages an app’s menus.

class NSMenuItem

A command item in an app menu.

class NSMenuItemBadge

A control that provides additional quantitative information specific to a menu item, such as the number of available updates.

protocol NSMenuDelegate

The optional methods implemented by delegates of NSMenu objects to manage menu display and handle some events.

### Menu Validation

protocol NSMenuItemValidation

### Menu Bar Items

class NSStatusBar

An object that manages a collection of status items displayed within the system-wide menu bar.

class NSStatusItem

An individual element displayed in the system menu bar.

class NSStatusBarButton

The appearance and behavior of an item in the systemwide menu bar.

### Cursors

class NSCursor

A pointer (also called a cursor).

class NSTrackingArea

A region of a view that generates mouse-tracking and cursor-update events when the pointer is over that region.

### The Dock

class NSDockTile

The visual representation of your app’s miniaturized windows and app icon as they appear in the Dock.

protocol NSDockTilePlugIn

A set of methods implemented by plug-ins that allow an app’s Dock tile to be customized while the app is not running.

## See Also

### User Interactions

Mouse, Keyboard, and Trackpad

Handle events related to mouse, keyboard, and trackpad input.

Gestures

Encapsulate your app’s event-handling logic in gesture recognizers so that you can reuse that code throughout your app.

Touch Bar

Display interactive content and controls in the Touch Bar.

Drag and Drop

Support the direct manipulation of your app’s content using drag and drop.

Accessibility for AppKit

Make your AppKit apps accessible to everyone who uses macOS.

