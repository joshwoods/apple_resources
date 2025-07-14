

- AppKit
- NSTableView
-  reloadData() 

Instance Method

# reloadData()

Marks the table view as needing redisplay, so it will reload the data for visible cells and draw the new values.

macOS

``` source
@MainActor
func reloadData()
```

## Discussion

This method forces a redraw of all the visible cells in the table view. If you want to update the value in a single cell, column, or row, it is more efficient to use frameOfCell(atColumn:row:), rect(ofColumn:), or rect(ofRow:) in conjunction with the setNeedsDisplay(_:) method of NSView. If you just want to update the scroller, use noteNumberOfRowsChanged(); if the height of a set of rows changes, use noteHeightOfRows(withIndexesChanged:).

Note

For NSView-based table views, this method drops all the visible row views and cell views, and re-acquires them all.

## See Also

### Related Documentation

func noteHeightOfRows(withIndexesChanged: IndexSet)

Informs the table view that the rows specified in `indexSet` have changed height.

func frameOfCell(atColumn: Int, row: Int) -> NSRect

Returns a rectangle locating the cell that lies at the intersection of the specified column and row.

func noteNumberOfRowsChanged()

Informs the table view that the number of records in its data source has changed.

func rect(ofColumn: Int) -> NSRect

Returns the rectangle containing the column at the specified index.

func rect(ofRow: Int) -> NSRect

Returns the rectangle containing the row at the specified index.

### Managing the Table’s Data

var dataSource: (any NSTableViewDataSource)?

The object that provides the data displayed by the table view.

var usesStaticContents: Bool

A Boolean value indicating whether the table uses static data.

func reloadData(forRowIndexes: IndexSet, columnIndexes: IndexSet)

Reloads the data for only the specified rows and columns.

