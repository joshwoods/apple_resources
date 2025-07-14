

- AppKit
- NSTableView
-  frameOfCell(atColumn:row:) 

Instance Method

# frameOfCell(atColumn:row:)

Returns a rectangle locating the cell that lies at the intersection of the specified column and row.

macOS

``` source
@MainActor
func frameOfCell(
    atColumn column: Int,
    row: Int
) -> NSRect
```

## Parameters 

`column`  

The index in the tableColumns array of the column containing the cell whose rectangle you want.

`row`  

The index of the row containing the cell whose rectangle you want.

## Return Value

A rectangle locating the cell that lies at the intersection of `columnIndex` and `rowIndex`. This method returns `NSZeroRect` if `columnIndex` or `rowIndex` is greater than the number of columns or rows in the table view.

## Discussion

You can use this method to update a single cell more efficiently than sending the table view a reloadData() message using reloadData(forRowIndexes:columnIndexes:)

The result of this method is used in a draw(withFrame:in:) message to the table column’s data cell. You can subclass and override this method to customize the frame of a particular cell. However, never return a frame larger than the default implementation returns.

The default frame is computed to have a height equal to the rect(ofRow:) for `rowIndex`, minus the half intercellSpacing height on the top and half on the bottom. The width of frame is equal to the with of the table column minus half the intercellSpacing width on the left, and half on the right.

## See Also

### Layout Support

var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection

The layout direction of the user interface.

func rect(ofColumn: Int) -> NSRect

Returns the rectangle containing the column at the specified index.

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

