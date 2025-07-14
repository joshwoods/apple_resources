

- Application Services
- Carbon Accessibility
-  Subroles 

API Collection

# Subroles

Define the values for an accessibility object’s subrole attribute.

## Overview

A subrole provides a more specific description of an accessibility object’s role. If an accessibility object is of a well-defined subtype, it can include the subrole attribute to provide additional information to an assistive application.

## Topics

### Constants

var kAXCloseButtonSubrole: String

A close button (that is, the red button in a window’s title bar that closes the window).

var kAXMinimizeButtonSubrole: String

A minimize button (that is, the yellow button in a window’s title bar that minimizes the window into the Dock).

var kAXZoomButtonSubrole: String

A zoom button (that is, the green button in a window’s title bar that adjusts the window’s size).

var kAXToolbarButtonSubrole: String

A toolbar button (that is, the button in a window’s title bar that hides and reveals the toolbar).

var kAXSecureTextFieldSubrole: String

A text field intended to contain sensitive data and that displays the user’s input as a series of bullets.

var kAXTableRowSubrole: String

A row in a table.

var kAXOutlineRowSubrole: String

A row in an outline view (see `kAXOutlineRole` for a description of an outline view).

var kAXUnknownSubrole: String

var kAXStandardWindowSubrole: String

A standard window that includes a title bar (that is, not an inspector window or a sheet).

var kAXDialogSubrole: String

A dialog window, such as an alert.

var kAXSystemDialogSubrole: String

A system-generated dialog window that floats on the top layer, regardless of which application is frontmost. Use this subrole only when a dialog or alert applies to the system as a whole, such as a shutdown dialog.

var kAXFloatingWindowSubrole: String

A utility window.

var kAXSystemFloatingWindowSubrole: String

A system-generated utility window.

var kAXIncrementArrowSubrole: String

The up arrow of a scroll bar.

var kAXDecrementArrowSubrole: String

The down arrow of a scroll bar.

var kAXIncrementPageSubrole: String

The increment area in the scroll track of a scroll bar.

var kAXDecrementPageSubrole: String

The decrement area in the scroll track of a scroll bar.

var kAXSortButtonSubrole: String

A column heading button in a list or column view.

var kAXSearchFieldSubrole: String

A search field.

var kAXApplicationDockItemSubrole: String

An icon in the Dock that represents an application.

var kAXDocumentDockItemSubrole: String

An icon in the Dock that represents a document.

var kAXFolderDockItemSubrole: String

An icon in the Dock that represents a folder.

var kAXMinimizedWindowDockItemSubrole: String

An icon in the Dock that represents a minimized window.

var kAXURLDockItemSubrole: String

An icon in the Dock that represents a URL.

var kAXDockExtraDockItemSubrole: String

An icon in the Dock that represents a Dock Extra.

var kAXTrashDockItemSubrole: String

The icon in the Dock that represents the Trash.

var kAXProcessSwitcherListSubrole: String

The display of running applications (processes) that appears when a user presses Command-Tab.

## See Also

### Accessibility Object Constants

Roles

Define the values an accessibility object’s role attribute can have.

Attributes

Define the attributes available for accessibility objects.

Parameterized Attributes

Define the parameterized attributes an accessibility object can have.

Actions

Define the actions an accessibility object can perform.

Notifications

Define the notifications that can be broadcast by an accessibility object.

Orientations and Sort Directions

Define the values for the orientation and sort-direction attributes of some accessibility objects.

