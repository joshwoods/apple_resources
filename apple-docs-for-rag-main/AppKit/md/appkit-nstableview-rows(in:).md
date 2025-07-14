

- AppKit
- NSTableView
-  rows(in:) 

Instance Method

# rows(in:)

Returns a range of indexes for the rows that lie wholly or partially within the vertical boundaries of the specified rectangle.

macOS

``` source
@MainActor
func rows(in rect: NSRect) -> NSRange
```

## Parameters 

`rect`  

A rectangle in the coordinate system of the table view.

## Return Value

A range of indexes for the table view’s rows that lie wholly or partially within the horizontal boundaries of `aRect`. If the width or height of `aRect` is `0`, this method returns an `NSRange` whose length is `0`.

## Discussion

The location of the range is the index of the first row in the rectangle, and the length is the number of rows that lie in the rectangle.

## See Also

### Layout Support

var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection

The layout direction of the user interface.

func rect(ofColumn: Int) -> NSRect

Returns the rectangle containing the column at the specified index.

func rect(ofRow: Int) -> NSRect

Returns the rectangle containing the row at the specified index.

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

