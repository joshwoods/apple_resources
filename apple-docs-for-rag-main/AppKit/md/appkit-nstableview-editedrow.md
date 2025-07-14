

- AppKit
- NSTableView
-  editedRow 

Instance Property

# editedRow

The index of the row being edited.

macOS

``` source
@MainActor
var editedRow: Int { get }
```

## Discussion

This property does not apply to view-based table views. In a view-based table view, the views are responsible for their own editing behavior. For other tables, the value reflects the index of the row being edited or `–1` when there is no editing session in progress.

## See Also

### Editing Cells

func editColumn(Int, row: Int, with: NSEvent?, select: Bool)

Edits the cell at the specified column and row using the specified event and selection behavior.

var editedColumn: Int

The index of the column being edited.

