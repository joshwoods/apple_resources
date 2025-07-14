

- AppKit
- NSTableView
-  rect(ofColumn:) 

Instance Method

# rect(ofColumn:)

Returns the rectangle containing the column at the specified index.

macOS

``` source
@MainActor
func rect(ofColumn column: Int) -> NSRect
```

## Parameters 

`column`  

The index in the tableColumns array of a column in the table view.

## Return Value

The rectangle containing the column at `columnIndex`. Returns `NSZeroRect` if `columnIndex` lies outside the range of valid column indexes for the table view.

## Discussion

You can use this method to update a single column more efficiently than sending the table view a reloadData() message.

```
[aTableView setNeedsDisplayInRect:[aTableView rectOfColumn:column]];
```

## See Also

### Related Documentation

func headerRect(ofColumn: Int) -> NSRect

Returns the rectangle containing the header tile for the column at `columnIndex`.

### Layout Support

var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection

The layout direction of the user interface.

func rect(ofRow: Int) -> NSRect

Returns the rectangle containing the row at the specified index.

func rows(in: NSRect) -> NSRange

Returns a range of indexes for the rows that lie wholly or partially within the vertical boundaries of the specified rectangle.

func columnIndexes(in: NSRect) -> IndexSet

Returns the indexes of the table view’s columns that intersect the specified rectangle.

func column(at: NSPoint) -> Int

Returns the index of the column the specified point lies in.

func row(at: NSPoint) -> Int

Returns the index of the row the specified point lies in.

func frameOfCell(atColumn: Int, row: Int) -> NSRect

Returns a rectangle locating the cell that lies at the intersection of the specified column and row.

var columnAutoresizingStyle: NSTableView.ColumnAutoresizingStyle

The table view’s column autoresizing style.

func sizeLastColumnToFit()

Resizes the last column so the table view fits exactly within its enclosing clip view.

func noteNumberOfRowsChanged()

Informs the table view that the number of records in its data source has changed.

func tile()

Properly sizes the table view and its header view and marks it as needing display.

func sizeToFit()

Sizes the table view based on a uniform column autoresizing style.

func noteHeightOfRows(withIndexesChanged: IndexSet)

Informs the table view that the rows specified in `indexSet` have changed height.

