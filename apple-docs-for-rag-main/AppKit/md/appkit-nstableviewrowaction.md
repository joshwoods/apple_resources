

- AppKit
-  NSTableViewRowAction 

Class

# NSTableViewRowAction

A single action to present when the user swipes horizontally on a table row.

macOS 10.11+

``` source
class NSTableViewRowAction
```

## Overview

In an editable table, performing a horizontal swipe on a row reveals a button to delete the row by default. This class lets you define one or more custom actions to display for a given row in your table. Each instance of this class represents a single action to perform and includes the text, formatting information, and behavior for the corresponding button.

To add custom actions to your table view’s rows, implement the tableView(_:rowActionsForRow:edge:) method in your table view’s delegate object. In that method, create and return an array of actions for the specified row. The table handles the remaining work of displaying the action buttons and executing the appropriate handler block when the user clicks the button.

## Topics

### Creating a Table Row Action

convenience init(style: NSTableViewRowAction.Style, title: String, handler: (NSTableViewRowAction, Int) -> Void)

Creates and returns a new table view row action object.

### Configuring the Action’s Appearance

var style: NSTableViewRowAction.Style

The style applied to the action button.

var title: String

The title of the action button.

var backgroundColor: NSColor!

The background color of the action button.

### Constants

enum Style

Constants that help define the appearance and behavior of action buttons.

### Instance Properties

var image: NSImage?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

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

struct ResizingOptions

