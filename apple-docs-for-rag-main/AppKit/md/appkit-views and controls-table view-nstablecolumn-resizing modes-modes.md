

- AppKit
- Views and Controls
- Table View
- NSTableColumn
-  Resizing Modes 

API Collection

# Resizing Modes

These constants specify the resizing modes for a table column. The values are used to set the resizingMask property.

## Topics

### Constants

static var autoresizingMask: NSTableColumn.ResizingOptions

Allows the table column to resize automatically in response to resizing the table view. The resizing behavior for the table view is set using the `NSTableView` method columnAutoresizingStyle.

static var userResizingMask: NSTableColumn.ResizingOptions

Allows the table column to be resized by the user.

