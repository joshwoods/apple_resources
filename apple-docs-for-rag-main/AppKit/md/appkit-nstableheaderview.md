

- AppKit
-  NSTableHeaderView 

Class

# NSTableHeaderView

An object that draws headers over a table view’s columns and handles mouse events in those headers.

macOS

``` source
@MainActor
class NSTableHeaderView
```

## Overview

NSTableHeaderView uses NSTableHeaderCell to implement its user interface.

## Topics

### Setting the table view

var tableView: NSTableView?

The NSTableView instance that this table header view belongs to.

### Checking altered columns

var draggedColumn: Int

The index of the column that the user is dragging.

var draggedDistance: CGFloat

The horizontal distance that the user has dragged a column.

var resizedColumn: Int

The index of the column that the user is resizing.

### Utility methods

func column(at: NSPoint) -> Int

Returns the index of the column whose header lies under `aPoint` in the receiver, or –1 if no such column is found.

func headerRect(ofColumn: Int) -> NSRect

Returns the rectangle containing the header tile for the column at `columnIndex`.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSViewToolTipOwner
- Sendable

## See Also

### Rows and Columns

class NSTableHeaderCell

An object that a table header view uses to draw the content of the column headers.

class NSTableRowView

The view shown for a row in a table view.

class NSTableColumn

The display characteristics and identifier for a column in a table view.

class NSTableViewRowAction

A single action to present when the user swipes horizontally on a table row.

struct ResizingOptions

