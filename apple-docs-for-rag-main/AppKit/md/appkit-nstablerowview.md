

- AppKit
-  NSTableRowView 

Class

# NSTableRowView

The view shown for a row in a table view.

macOS 10.7+

``` source
@MainActor
class NSTableRowView
```

## Overview

NSTableRowView is responsible for displaying attributes associated with the row, including the selection highlight, and group row look.

## Topics

### Display Style

var isEmphasized: Bool

Determines whether the row will draw with the alternate or secondary color (unless overridden).

var interiorBackgroundStyle: NSView.BackgroundStyle

Specifies how the subviews should draw.

var isFloating: Bool

Specifies whether the row is drawn using the floating style.

### Row Selection

var isSelected: Bool

Determines whether the row is selected.

var selectionHighlightStyle: NSTableView.SelectionHighlightStyle

Specifies the selection highlight style.

### Drag and Drop

var draggingDestinationFeedbackStyle: NSTableView.DraggingDestinationFeedbackStyle

Specifies the dragging destination feedback style.

var indentationForDropOperation: CGFloat

Defines the amount the drag target for a row should be indented.

var isTargetForDropOperation: Bool

Specifies whether this row will draw a drop indicator based on the current dragging feedback style.

### Row Grouping

var isGroupRowStyle: Bool

Specifies whether this row view is a group row.

var numberOfColumns: Int

Returns the number of columns represented by views in the table row view.

### Overriding Row View Display Characteristics

var backgroundColor: NSColor

The background color of the row.

func drawBackground(in: NSRect)

Draws the background of the row in the rectangle.

func drawDraggingDestinationFeedback(in: NSRect)

Draws the row’s dragging destination feedback when the entire row is a drop target.

func drawSelection(in: NSRect)

Draws the selected row.

func drawSeparator(in: NSRect)

Draws the horizontal separator between table rows.

### Accessing A Row Column View

func view(atColumn: Int) -> Any?

Provides access to the given view at a particular column.

### Instance Properties

var isNextRowSelected: Bool

var isPreviousRowSelected: Bool

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
- NSAccessibilityGroup
- NSAccessibilityProtocol
- NSAccessibilityRow
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Rows and Columns

class NSTableHeaderView

An object that draws headers over a table view’s columns and handles mouse events in those headers.

class NSTableHeaderCell

An object that a table header view uses to draw the content of the column headers.

class NSTableColumn

The display characteristics and identifier for a column in a table view.

class NSTableViewRowAction

A single action to present when the user swipes horizontally on a table row.

struct ResizingOptions

