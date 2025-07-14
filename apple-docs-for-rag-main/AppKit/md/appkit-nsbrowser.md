

- AppKit
-  NSBrowser 

Class

# NSBrowser

An interface that displays a hierarchically organized list of data items that can be navigated and selected.

macOS

``` source
@MainActor
class NSBrowser
```

## Overview

A browser displays information using a set of columns, which are indexed from left to right. Each successive column displays the next level down in the data hierarchy. This class uses the NSBrowserCell class to implement its user interface.

Browsers have the following components:

- Columns

- Scroll views

- Matrices

- Browser cells

To the user, browsers display data in columns and rows within each column. These components are arranged in the following component hierarchy:

```
Browser
|---Columns [1..*]
    |---Scroll view
       |---Matrix
           |---Rows [0..*]
```

### Superclass overrides

- isOpaque returns true when the browser doesn’t have a title and its background color’s alpha component is `1.0`; otherwise, it returns false.

### Protocol implementations

- The NSBrowser implementation of namesOfPromisedFilesDropped(atDestination:) provides the names of the files that the browser promises to create at a specified location, the result of sending `browser:namesOfPromisedFilesDroppedAtDestination:forDraggedRowsWithIndexes:inColumn:` to the delegate.

## Topics

### Configuring Browsers

var reusesColumns: Bool

A Boolean that indicates whether the browser reuses matrix objects after their columns are unloaded.

var maxVisibleColumns: Int

The maximum number of visible columns.

var autohidesScroller: Bool

A Boolean that indicates whether the browser automatically hides its scroller.

var backgroundColor: NSColor

The browser’s background color.

var minColumnWidth: CGFloat

The minimum column width, in pixels.

var separatesColumns: Bool

A Boolean that indicates whether columns are separated by bezeled borders.

var takesTitleFromPreviousColumn: Bool

A Boolean that indicates whether a column takes its title from the selected cell in the previous column.

func tile()

Adjusts the various subviews of the browser—scrollers, columns, titles, and so on—without redrawing.

var delegate: (any NSBrowserDelegate)?

The browser’s delegate.

### Managing Component Types

class var cellClass: AnyClass

Returns the `NSBrowserCell` class.

func setCellClass(AnyClass)

Sets the class of the cell to be used by the matrices in the columns of the browser.

var cellPrototype: Any!

The prototype `NSCell` for displaying items in the matrices in the columns of the browser.

### Managing Selection Behavior

var allowsBranchSelection: Bool

A Boolean that indicates whether the user can select branch items.

var allowsEmptySelection: Bool

A Boolean that indicates whether there can be nothing selected.

var allowsMultipleSelection: Bool

A Boolean that indicates whether the user can select multiple items.

func selectedRowIndexes(inColumn: Int) -> IndexSet?

Provides the indexes of the selected rows in a given column of the browser.

func selectRowIndexes(IndexSet, inColumn: Int)

Specifies the selected rows in a given column of the browser.

var allowsTypeSelect: Bool

A Boolean that indicates whether the browser allows keystroke-based selection (type select).

### Managing Selection

func selectedCell(inColumn: Int) -> Any?

Returns the last (lowest) cell selected in the given column.

var selectedCells: [NSCell]?

All cells selected in the rightmost column.

func selectAll(Any?)

Selects all cells in the last column of the browser.

func selectedRow(inColumn: Int) -> Int

Returns the row index of the selected cell in the specified column.

func selectRow(Int, inColumn: Int)

Selects the cell at the specified row and column index.

var selectionIndexPath: IndexPath?

The index path of the item selected in the browser.

var selectionIndexPaths: [IndexPath]

An array containing the index paths of all items selected in the browser.

### Accessing Components

func loadedCell(atRow: Int, column: Int) -> Any?

Loads, if necessary, and returns the cell at the specified row and column location.

func editItem(at: IndexPath, with: NSEvent?, select: Bool)

Begins editing the item at the specified path.

func item(at: IndexPath) -> Any?

Returns the item at the specified index path.

func item(atRow: Int, inColumn: Int) -> Any?

Returns the item located at the specified row and column.

func indexPath(forColumn: Int) -> IndexPath

Returns the index path of the item whose children are displayed in the given column.

func isLeafItem(Any?) -> Bool

Returns whether the specified item is a leaf item.

func parentForItems(inColumn: Int) -> Any?

Returns the item that contains the children located in the specified column.

### Managing the Path

func path() -> String

Returns a string representing the browser’s current path.

func setPath(String) -> Bool

Sets the path to be displayed by the browser.

func path(toColumn: Int) -> String

Returns a string representing the path from the first column up to, but not including, the column at the given index.

var pathSeparator: String

The path separator.

### Managing Columns

func addColumn()

Adds a column to the right of the last column.

var selectedColumn: Int

The index of the last column with a selected item.

var lastColumn: Int

The index of the last column loaded.

var firstVisibleColumn: Int

The index of the first visible column.

var numberOfVisibleColumns: Int

The number of visible columns.

var lastVisibleColumn: Int

The index of the last visible column.

func validateVisibleColumns()

Validates the browser’s visible columns.

var isLoaded: Bool

A Boolean that indicates whether column 0 is loaded.

func loadColumnZero()

Loads column 0; unloads previously loaded columns.

func reloadColumn(Int)

Reloads the given column.

### Accessing Column Titles

func title(ofColumn: Int) -> String?

Returns the title displayed for the given column.

func setTitle(String, ofColumn: Int)

Sets the title of the given column.

var isTitled: Bool

A Boolean that indicates whether columns display titles.

func drawTitle(ofColumn: Int, in: NSRect)

Draws the title for the specified column within the given rectangle.

var titleHeight: CGFloat

The height of the column titles for the browser.

func titleFrame(ofColumn: Int) -> NSRect

Returns the bounds of the title frame for the specified column.

### Updating Browsers

func noteHeightOfRowsWithIndexesChanged(IndexSet, inColumn: Int)

Immediately retiles the browser’s columns using row heights specified by the browser’s delegate.

func reloadData(forRowIndexes: IndexSet, inColumn: Int)

Updates the rows in the column with the specified column index with indexes in the specified set.

### Scrolling

var hasHorizontalScroller: Bool

A Boolean that indicates whether the browser has a horizontal scroller.

func scrollColumnToVisible(Int)

Scrolls to make the specified column visible.

func scrollColumnsLeft(by: Int)

Scrolls columns left by the specified number of columns.

func scrollColumnsRight(by: Int)

Scrolls columns right by the specified number of columns.

func scrollRowToVisible(Int, inColumn: Int)

Scrolls the specified row to be visible within the specified column.

### Dragging

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Specifies the drag-operation mask for dragging operations with local or external destinations.

func canDragRows(with: IndexSet, inColumn: Int, with: NSEvent) -> Bool

Indicates whether the browser can attempt to initiate a drag of the given rows for the given event.

func draggingImageForRows(with: IndexSet, inColumn: Int, with: NSEvent, offset: NSPointPointer?) -> NSImage?

Provides an image to represent dragged rows during a drag operation on the browser.

### Getting Column Frames

func frame(ofColumn: Int) -> NSRect

Returns the rectangle containing the given column.

func frame(ofInsideOfColumn: Int) -> NSRect

Returns the rectangle containing the specified column, not including borders.

### Getting Row Frames

func frame(ofRow: Int, inColumn: Int) -> NSRect

Returns the frame of the cell at the specified location, including the expandable arrow.

func getRow(UnsafeMutablePointer&lt;Int>?, column: UnsafeMutablePointer&lt;Int>?, for: NSPoint) -> Bool

Gets the row and column coordinates for the specified point, if a cell exists at that point.

### Managing Actions

var doubleAction: Selector?

The browser’s double-click action method.

var sendsActionOnArrowKeys: Bool

A Boolean that indicates whether pressing an arrow key causes an action message to be sent.

func sendAction() -> Bool

Sends the action message to the target.

### Handling Mouse-Click Events

func doClick(Any?)

Responds to (single) mouse clicks in a column of the browser.

func doDoubleClick(Any?)

Responds to double clicks in a column of the browser.

var clickedColumn: Int

The column number of the cell that the user clicked to display a context menu.

var clickedRow: Int

The row number of the cell that the user clicked to display a context menu.

### Sizing

class func removeSavedColumns(withAutosaveName: NSBrowser.ColumnsAutosaveName)

Removes the column configuration data stored under the given name from the application’s user defaults.

var columnsAutosaveName: NSBrowser.ColumnsAutosaveName

The name used to automatically save the browser’s column configuration.

typealias ColumnsAutosaveName

func columnContentWidth(forColumnWidth: CGFloat) -> CGFloat

Returns the content width for a given column width.

func columnWidth(forColumnContentWidth: CGFloat) -> CGFloat

Returns the column width for the width of the given column’s content.

var columnResizingType: NSBrowser.ColumnResizingType

A constant indicating the browser’s column resizing type.

var prefersAllColumnUserResizing: Bool

A Boolean that indicates whether the browser is set to resize all columns simultaneously rather than resizing a single column at a time.

func width(ofColumn: Int) -> CGFloat

Returns the width of the specified column.

func setWidth(CGFloat, ofColumn: Int)

Sets the width of the specified column.

func defaultColumnWidth() -> CGFloat

Returns the default column width of the browser’s columns.

func setDefaultColumnWidth(CGFloat)

Sets the default column width for new browser columns that do not otherwise have an initial width from defaults or the browser’s delegate.

var rowHeight: CGFloat

The height of the browser’s rows.

### Constants

enum ColumnResizingType

Types of browser column resizing.

enum DropOperation

The type used to specify the drop type of a drag-and-drop operation. See browser(_:validateDrop:proposedRow:column:dropOperation:) for more information.

Application Kit Versions for NSBrowser Functionality

The version of the AppKit.framework containing a specific bug fix or capability.

### Notifications

class let columnConfigurationDidChangeNotification: NSNotification.Name

Notifies the delegate when the width of a browser column has changed.

### Deprecated

func column(of: NSMatrix) -> Int

Returns the column number in which the given matrix is located.

Deprecated

func matrix(inColumn: Int) -> NSMatrix?

Returns the matrix located in the specified column.

Deprecated

func matrixClass() -> AnyClass

Returns the matrix class used in the browser’s columns.

Deprecated

func setMatrixClass(AnyClass)

Sets the matrix class to be used in the browser’s columns.

Deprecated

### Instance Methods

func selectedCell() -> Any?

## Relationships

### Inherits From

- NSControl

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

