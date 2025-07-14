

- AppKit
- NSTableView
-  editColumn(\_:row:with:select:) 

Instance Method

# editColumn(\_:row:with:select:)

Edits the cell at the specified column and row using the specified event and selection behavior.

macOS

``` source
@MainActor
func editColumn(
    _ column: Int,
    row: Int,
    with event: NSEvent?,
    select: Bool
)
```

## Parameters 

`column`  

The index of the column in the tableColumns array.

`row`  

The row index.

`event`  

The event.

`select`  

true if the entered contents should be selected, otherwise false.

## Discussion

This method is invoked automatically in response to user actions; you should rarely need to invoke it directly. `theEvent` is usually the mouse event that triggered editing; it can be `nil` when starting an edit programmatically.

This method scrolls the table view so that the cell is visible and sets up the field editor. If `flag` is false, it calls the edit(withFrame:in:editor:delegate:event:) method of the field editor’s NSCell object, providing the `NSTableView` as the text delegate. If `flag` is true, this method calls the select(withFrame:in:editor:delegate:start:length:) method instead.

This method can be overridden to customize drawing for `rowIndex` when using NSCell-based table views.

Note

When using NSView-based table views, this method attempts to make the view at the specified `column` and `row` the first responder, which will begin editing if the view supports editing. This method should not be subclassed or overridden for NSView-based table views. Instead, row drawing customization can be done by subclassing NSTableRowView.

## See Also

### Editing Cells

var editedColumn: Int

The index of the column being edited.

var editedRow: Int

The index of the row being edited.

