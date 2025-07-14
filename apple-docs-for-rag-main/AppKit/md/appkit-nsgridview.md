

- AppKit
-  NSGridView 

Class

# NSGridView

A container that aligns views in a flexible grid of rows and columns.

macOS 10.12+

``` source
@MainActor
class NSGridView
```

## Overview

A grid view helps you lay out content, such as photos or thumbnails, in a row-column arrangement similar to a spreadsheet. Within a grid view, an item that occupies a single row-column intersection is represented by an NSGridCell object.

## Topics

### Creating a Grid View

convenience init(numberOfColumns: Int, rows: Int)

Creates a newly allocated grid view object with the specified number of columns and rows.

convenience init(views: [[NSView]])

Creates a newly allocated grid view object with the specified array of arrays of views.

init(frame: NSRect)

Creates a newly allocated grid view object with the specified frame rectangle.

init?(coder: NSCoder)

Creates a newly allocated grid view object from the coder.

### Getting Information About the Grid

var numberOfRows: Int

The number of rows in the grid view.

var numberOfColumns: Int

The number of columns in the grid view.

func index(of: NSGridColumn) -> Int

Returns the index of the specified grid column.

func row(at: Int) -> NSGridRow

Returns the grid row object at the specified index.

func column(at: Int) -> NSGridColumn

Returns the grid column object at the specified index.

func index(of: NSGridRow) -> Int

Returns the index of the specified grid row.

### Adding, Removing, and Moving Rows

func addRow(with: [NSView]) -> NSGridRow

Adds an array of views to a new row.

func insertRow(at: Int, with: [NSView]) -> NSGridRow

Inserts the array of view objects into the grid view at the index.

func removeRow(at: Int)

Removes the row from the grid view at the index.

func moveRow(at: Int, to: Int)

Moves the specified row to the new row location.

### Adding, Removing, and Moving Columns

func addColumn(with: [NSView]) -> NSGridColumn

Adds a new column containing the array of views.

func insertColumn(at: Int, with: [NSView]) -> NSGridColumn

Inserts the array of view objects at the specified index.

func removeColumn(at: Int)

Removes the column from the grid view at the specified index.

func moveColumn(at: Int, to: Int)

Moves the specified column to a new column location.

### Managing Grid Spacing and Alignment

class let sizedForContent: CGFloat

The default value for row and column sizes.

var columnSpacing: CGFloat

The column spacing for the grid view.

var rowSpacing: CGFloat

The row spacing for the grid view.

var rowAlignment: NSGridRow.Alignment

The row alignment for the grid view.

var xPlacement: NSGridCell.Placement

The placement of the cell within the grid column.

var yPlacement: NSGridCell.Placement

The placement of the cell within the grid row.

### Creating and Merging Cells

func cell(atColumnIndex: Int, rowIndex: Int) -> NSGridCell

Returns the grid cell object at the specified column and row index.

func cell(for: NSView) -> NSGridCell?

Returns the grid cell object that contains the given view or one of its ancestors.

func mergeCells(inHorizontalRange: NSRange, verticalRange: NSRange)

Expands the cell at the top-leading corner of the horizontal and vertical range to cover the entire area.

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
- Sendable

