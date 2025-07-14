

- AppKit
-  NSMatrix 

Class

# NSMatrix

A legacy interface for grouping radio buttons or other types of cells together.

macOS

``` source
@MainActor
class NSMatrix
```

## Overview

Important

Use of NSMatrix is discouraged in apps that run in macOS 10.8 and later. If you need to create a radio button group in an app that runs in macOS 10.8 and later, create instances of NSButton that each specify a button type of `NSRadioButton` and specify the same action and the same superview for each button in the group.

`NSMatrix` uses flipped coordinates by default. The cells in an NSMatrix object are numbered by row and column, each starting with 0; for example, the top left NSCell would be at (0, 0), and the NSCell that’s second down and third across would be at (1, 2).

The NSMatrix class has the notion of a single selected cell, which is the cell that was most recently clicked or that was so designated by a selectCell(atRow:column:) or selectCell(withTag:) message. The selected cell is the cell chosen for action messages except for performClick(_:) (NSCell), which is assigned to the key cell. (The key cell is generally identical to the selected cell, but can be given click focus while leaving the selected cell unchanged.) If the user has selected multiple cells, the selected cell is the one lowest and furthest to the right in the matrix of cells.

## Topics

### Initializing an NSMatrix Object

convenience init(frame: NSRect)

Initializes a newly allocated matrix with the specified frame.

init(frame: NSRect, mode: NSMatrix.Mode, cellClass: AnyClass?, numberOfRows: Int, numberOfColumns: Int)

Initializes and returns a newly allocated matrix of the specified size using cells of the given class.

init(frame: NSRect, mode: NSMatrix.Mode, prototype: NSCell, numberOfRows: Int, numberOfColumns: Int)

Initializes and returns a newly allocated matrix of the specified size using the given cell as a prototype.

### Configuring the Matrix Object

var mode: NSMatrix.Mode

The selection mode of the receiver.

var allowsEmptySelection: Bool

A Boolean that indicates whether a radio-mode matrix supports an empty selection.

var isSelectionByRect: Bool

A Boolean that indicates whether the user can select a rectangle of cells in the receiver by dragging the cursor.

### Managing the Cell Class

var cellClass: AnyClass

The subclass of NSCell that the matrix uses when creating new (empty) cells.

var prototype: NSCell?

The prototype cell that’s copied whenever the matrix creates a new cell.

### Laying Out the Cells of the Matrix

func addColumn()

Adds a new column of cells to the right of the last column.

func addColumn(with: [NSCell])

Adds a new column of cells to the right of the last column, using the given cells.

func addRow()

Adds a new row of cells below the last row.

func addRow(with: [NSCell])

Adds a new row of cells below the last row, using the specified cells.

func cellFrame(atRow: Int, column: Int) -> NSRect

Returns the frame rectangle of the cell that would be drawn at the specified location.

var cellSize: NSSize

The size of each cell in the matrix.

func getNumberOfRows(UnsafeMutablePointer&lt;Int>?, columns: UnsafeMutablePointer&lt;Int>?)

Obtains the number of rows and columns in the receiver.

func insertColumn(Int)

Inserts a new column of cells at the specified location. .

func insertColumn(Int, with: [NSCell]?)

Inserts a new column of cells before the specified column, using the given cells.

func insertRow(Int)

Inserts a new row of cells before the specified row.

func insertRow(Int, with: [NSCell]?)

Inserts a new row of cells before the specified row, using the given cells.

var intercellSpacing: NSSize

The vertical and horizontal spacing between cells in the matrix.

func makeCell(atRow: Int, column: Int) -> NSCell

Creates a new cell at the location specified by the given row and column in the receiver.

var numberOfColumns: Int

The number of columns in the matrix.

var numberOfRows: Int

The number of rows in the matrix.

func putCell(NSCell, atRow: Int, column: Int)

Replaces the cell at the specified row and column with the new cell.

func removeColumn(Int)

Removes the specified column at from the receiver.

func removeRow(Int)

Removes the specified row from the receiver.

func renewRows(Int, columns: Int)

Changes the number of rows and columns in the receiver.

func sort(using: (Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?)

Sorts the receiver’s cells in ascending order as defined by the specified comparison function.

func sort(using: Selector)

Sorts the receiver’s cells in ascending order as defined by the comparison method.

### Auto Layout Sizing

var autorecalculatesCellSize: Bool

A Boolean that indicates whether the matrix auto-recalculates its cell size.

### Finding Matrix Coordinates

func getRow(UnsafeMutablePointer&lt;Int>, column: UnsafeMutablePointer&lt;Int>, for: NSPoint) -> Bool

Indicates whether the specified point lies within one of the cells of the matrix and returns the location of the cell within which the point lies.

func getRow(UnsafeMutablePointer&lt;Int>, column: UnsafeMutablePointer&lt;Int>, of: NSCell) -> Bool

Searches the receiver for the specified cell and returns the row and column of the cell

### Managing Attributes of Individual Cells

func setState(Int, atRow: Int, column: Int)

Sets the state of the cell at specified location.

func setToolTip(String?, for: NSCell)

Sets the tooltip for the cell.

func toolTip(for: NSCell) -> String?

Returns the tooltip for the specified cell.

### Selecting and Deselecting Cells

func selectCell(atRow: Int, column: Int)

Selects the cell at the specified row and column within the receiver.

func selectCell(withTag: Int) -> Bool

Selects the last cell with the given tag.

func selectAll(Any?)

Selects and highlights all cells in the receiver.

var keyCell: NSCell?

The cell that will be clicked when the user presses the Space bar.

func setSelectionFrom(Int, to: Int, anchor: Int, highlight: Bool)

Programmatically selects a range of cells.

func deselectAllCells()

Deselects all cells in the receiver and, if necessary, redisplays the receiver.

func deselectSelectedCell()

Deselects the selected cell or cells.

### Finding Cells

var selectedCells: [NSCell]

An array containing all of the matrix’s highlighted cells plus its selected cell.

var selectedColumn: Int

The column number of the selected cell.

var selectedRow: Int

The row number of the selected cell.

func cell(atRow: Int, column: Int) -> NSCell?

Returns the cell at the specified row and column.

func cell(withTag: Int) -> NSCell?

Searches the receiver and returns the last cell matching the specified tag.

var cells: [NSCell]

An array containing the cells of the matrix.

### Modifying Graphics Attributes

var backgroundColor: NSColor

The background color of the matrix (the space between the cells).

var cellBackgroundColor: NSColor?

The background color of the matrix’s cells.

var drawsBackground: Bool

A Boolean that indicates whether the matrix draws its background.

var drawsCellBackground: Bool

A Boolean that indicates whether the matrix draws the background within each of its cells.

### Editing Text in Cells

func selectText(Any?)

Selects text in the currently selected cell or in the key cell.

func selectText(atRow: Int, column: Int) -> NSCell?

Selects the text in the cell at the specified location and returns the cell.

func textShouldBeginEditing(NSText) -> Bool

Requests permission to begin editing text.

func textDidBeginEditing(Notification)

Invoked when there’s a change in the text after the receiver gains first responder status.

func textDidChange(Notification)

Invoked when a key-down event or paste operation occurs that changes the receiver’s contents.

func textShouldEndEditing(NSText) -> Bool

Requests permission to end editing.

func textDidEndEditing(Notification)

Invoked when text editing ends.

### Setting Tab Key Behavior

var tabKeyTraversesCells: Bool

A Boolean that indicates whether pressing the Tab key advances the key cell to the next selectable cell.

### Managing the Delegate

var delegate: (any NSMatrixDelegate)?

The delegate for messages from the field editor.

protocol NSMatrixDelegate

The `NSMatrixDelegate` protocol defines the optional methods implemented by delegates of `NSMatrix` objects.

### Resizing the Matrix and Its Cells

var autosizesCells: Bool

A Boolean that indicates whether the cell sizes change when the receiver is resized.

func setValidateSize(Bool)

Specifies whether the receiver’s size information is validated.

func sizeToCells()

Changes the width and the height of the receiver’s frame so it exactly contains the cells.

### Scrolling Cells in the Matrix

var isAutoscroll: Bool

A Boolean that indicates whether the receiver is automatically scrolled.

func setScrollable(Bool)

Specifies whether the cells in the matrix are scrollable.

func scrollCellToVisible(atRow: Int, column: Int)

Scrolls the receiver so the specified cell is visible.

### Displaying and Highlighting Cells

func drawCell(atRow: Int, column: Int)

Displays the cell at the specified row and column.

func highlightCell(Bool, atRow: Int, column: Int)

Highlights or unhighlights the cell at the specified row and column location.

### Managing and Sending Action Messages

func sendAction() -> Bool

If the selected cell has both an action and a target, sends its action to its target.

func sendAction(Selector, to: Any, forAllCells: Bool)

Iterates through the cells in the receiver, sending the specified selector to an object for each cell.

var doubleAction: Selector?

The action sent to the target of the receiver when the user double-clicks a cell.

func sendDoubleAction()

Sends the double-click action message to the target of the receiver.

### Handling Event and Action Messages

func acceptsFirstMouse(for: NSEvent?) -> Bool

Returns a Boolean value indicating whether the receiver accepts the first mouse.

func mouseDown(with: NSEvent)

Responds to a mouse-down event.

var mouseDownFlags: Int

The flags in effect at the mouse-down event that started the current tracking session.

func performKeyEquivalent(with: NSEvent) -> Bool

Looks for a cell that has the given key equivalent and, if found, makes that cell respond as if clicked.

### Managing the Cursor

func resetCursorRects()

Resets cursor rectangles so the cursor becomes an I-beam over text cells.

### Constants

enum Mode

These constants determine how NSCell objects behave when an NSMatrix object is tracking the mouse.

### Instance Methods

func selectedCell() -> NSCell?

## Relationships

### Inherits From

- NSControl

### Inherited By

- NSForm

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
- NSUserInterfaceValidations
- NSViewToolTipOwner
- Sendable

## See Also

### Controls

Responding to control-based events using target-action

Handle user input by connecting buttons, sliders, and other controls to your app’s code using the target-action design pattern.

class NSButton

A control that defines an area on the screen that a user clicks to trigger an action.

class NSColorWell

A control that displays a color value and lets the user change that color value.

Combo Box

Display a list of values in a pop-up menu that lets the user select a value or type in a custom value.

class NSComboButton

A button with a pull-down menu and a default action.

Date Picker

Display a calendar date and provide controls for editing the date value.

class NSImageView

A display of image data in a frame.

class NSLevelIndicator

A visual representation of a level or quantity, using discrete values.

Path Control

A display of a file system path or virtual path information.

class NSPopUpButton

A control for selecting an item from a list.

class NSProgressIndicator

An interface that provides visual feedback to the user about the status of an ongoing task.

class NSRuleEditor

An interface for configuring a rule-based list of options.

class NSPredicateEditor

A defined set of rules that allows the editing of predicate objects.

Search Field

Provide a text field that is optimized for text-based search interfaces.

class NSSegmentedControl

Display one or more buttons in a single horizontal group.

