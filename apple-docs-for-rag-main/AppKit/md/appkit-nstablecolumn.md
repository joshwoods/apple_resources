

- AppKit
-  NSTableColumn 

Class

# NSTableColumn

The display characteristics and identifier for a column in a table view.

macOS

``` source
@MainActor
class NSTableColumn
```

## Overview

A table column object determines the width (including the maximum and minimum widths) of its column in the table view and specifies the column’s resizing and editing behavior. A table column stores two cell objects: the header cell, which is used to draw the column header, and the data cell, which is used to draw the values for each row. In a cell-based table, you can control the display of the column by specifying subclasses of `NSCell` to use and by setting the font and other display characteristics for these cells. For example, you can use an NSTextFieldCell to display string values or substitute an NSImageCell to display pictures.

## Topics

### Creating a Table Column

init(identifier: NSUserInterfaceItemIdentifier)

Initializes a newly created table column with a string identifier.

### Setting the Table View

var tableView: NSTableView?

The table view that contains the table column.

### Controlling Size

var width: CGFloat

The table column’s width, in points.

var minWidth: CGFloat

The table column’s minimum width, in points.

var maxWidth: CGFloat

The table column’s maximum width, in points.

var resizingMask: NSTableColumn.ResizingOptions

The table column’s resizing mask.

func sizeToFit()

Resizes the table column to fit the width of its header cell.

### Setting the Header

var title: String

The title of the table column’s header.

var headerCell: NSTableHeaderCell

The cell used to draw the table column’s header.

### Setting the Identifier

var identifier: NSUserInterfaceItemIdentifier

The identifier string for the table column.

### Controlling Editability in a Cell-Based Table

var isEditable: Bool

A Boolean that indicates whether a cell-based table’s column cells are user editable.

### Sorting

var sortDescriptorPrototype: NSSortDescriptor?

The table column’s sort descriptor prototype.

### Setting Column Visibility

var isHidden: Bool

A Boolean that indicates whether the table column is hidden.

### Setting Tooltips

var headerToolTip: String?

The string that’s displayed in a help tag over the table column header.

### Deprecated Methods

var dataCell: Any

The cell prototype used by the table column to draw individual cells.

Deprecated

func dataCell(forRow: Int) -> Any

Returns the cell object used to display values in the specified row of the table column.

Deprecated

### Constants

Resizing Modes

These constants specify the resizing modes for a table column. The values are used to set the resizingMask property.

### Initializers

init(coder: NSCoder)

### Structures

struct ResizingOptions

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Rows and Columns

class NSTableHeaderView

An object that draws headers over a table view’s columns and handles mouse events in those headers.

class NSTableHeaderCell

An object that a table header view uses to draw the content of the column headers.

class NSTableRowView

The view shown for a row in a table view.

class NSTableViewRowAction

A single action to present when the user swipes horizontally on a table row.

struct ResizingOptions

