

- AppKit
- NSTableColumn
-  dataCell(forRow:) Deprecated

Instance Method

# dataCell(forRow:)

Returns the cell object used to display values in the specified row of the table column.

macOS

``` source
@MainActor
func dataCell(forRow row: Int) -> Any
```

Deprecated

Cell-based table views are deprecated; use view-based table views instead. See view(atColumn:row:makeIfNecessary:).

## Parameters 

`row`  

The table column row.

## Return Value

The data cell object.

## Discussion

Returns the NSCell object used by the table view to draw values for the receiver. The table view calls this method when drawing the row, so you shouldn’t need to call it directly. By default, this method just accesses dataCell.

To enable per-row customization of the cell used by the table column, you can override this method or use the `NSTableViewDelegate` method tableView(_:dataCellFor:row:). In both cases, the cell that’s returned should properly implement copy(with:), because the table view may copy the cell during certain operations.

Subclasses should be prepared for this method to be called with `row` equal to –1 in cases where no actual row is involved but the table view needs to get some generic cell information.

Note

This method is only valid for cell-based table views.

## See Also

### Deprecated Methods

var dataCell: Any

The cell prototype used by the table column to draw individual cells.

Deprecated

