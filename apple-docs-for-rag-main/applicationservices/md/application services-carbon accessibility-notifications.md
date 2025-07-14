

- Application Services
- Carbon Accessibility
-  Notifications 

API Collection

# Notifications

Define the notifications that can be broadcast by an accessibility object.

## Topics

### Constants

var kAXMainWindowChangedNotification: String

The main window has changed.

var kAXFocusedWindowChangedNotification: String

The focused window has changed.

var kAXFocusedUIElementChangedNotification: String

The focused accessibility object has changed.

var kAXApplicationActivatedNotification: String

The application was activated (that is, brought to front).

var kAXApplicationDeactivatedNotification: String

The application was deactivated.

var kAXApplicationHiddenNotification: String

The application was hidden.

var kAXApplicationShownNotification: String

The application was shown (that is, a hidden application is now visible).

var kAXWindowCreatedNotification: String

A window was created. Carbon automatically sends this notification when window is created, as long as the window is implemented using Carbon window mechanisms.

var kAXWindowMovedNotification: String

The window was moved (this notification is sent at the end of the window-move operation, not during it).

var kAXWindowResizedNotification: String

The window was resized (this notification is sent at the end of the window-resize operation, not during it).

var kAXWindowMiniaturizedNotification: String

The application was minimized (that is, moved into the Dock).

var kAXWindowDeminiaturizedNotification: String

The window was moved out of the Dock.

var kAXDrawerCreatedNotification: String

A drawer was created (that is, a drawer now extends from this window).

var kAXSheetCreatedNotification: String

A sheet was created (that is, a modal dialog now extends from this window).

var kAXHelpTagCreatedNotification: String

A help tag is now visible for this accessibility object.

var kAXValueChangedNotification: String

The value of an accessibility object’s value attribute was changed.

var kAXUIElementDestroyedNotification: String

An accessibility object was disposed of.

var kAXMenuOpenedNotification: String

A menu was opened.

var kAXMenuClosedNotification: String

A menu was closed.

var kAXMenuItemSelectedNotification: String

A menu item was selected.

var kAXRowCountChangedNotification: String

The number of rows in this table was changed.

var kAXSelectedChildrenChangedNotification: String

A different subset of this accessibility object’s children were selected.

var kAXResizedNotification: String

The window has changed size.

var kAXMovedNotification: String

The position of this accessibility object was changed.

var kAXCreatedNotification: String

An accessibility object was created.

## See Also

### Accessibility Object Constants

Roles

Define the values an accessibility object’s role attribute can have.

Subroles

Define the values for an accessibility object’s subrole attribute.

Attributes

Define the attributes available for accessibility objects.

Parameterized Attributes

Define the parameterized attributes an accessibility object can have.

Actions

Define the actions an accessibility object can perform.

Orientations and Sort Directions

Define the values for the orientation and sort-direction attributes of some accessibility objects.

