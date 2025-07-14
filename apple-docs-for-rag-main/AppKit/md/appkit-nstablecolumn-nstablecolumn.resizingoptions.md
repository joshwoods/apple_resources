

- AppKit
- NSTableColumn
-  NSTableColumn.ResizingOptions 

Structure

# NSTableColumn.ResizingOptions

macOS

``` source
struct ResizingOptions
```

## Topics

### Initializers

init(rawValue: UInt)

### Constants

static var autoresizingMask: NSTableColumn.ResizingOptions

Allows the table column to resize automatically in response to resizing the table view. The resizing behavior for the table view is set using the `NSTableView` method columnAutoresizingStyle.

static var userResizingMask: NSTableColumn.ResizingOptions

Allows the table column to be resized by the user.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Rows and Columns

class NSTableHeaderView

An object that draws headers over a table view’s columns and handles mouse events in those headers.

class NSTableHeaderCell

An object that a table header view uses to draw the content of the column headers.

class NSTableRowView

The view shown for a row in a table view.

class NSTableColumn

The display characteristics and identifier for a column in a table view.

class NSTableViewRowAction

A single action to present when the user swipes horizontally on a table row.

