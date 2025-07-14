

- AppKit
- NSTableView
-  userInterfaceLayoutDirection 

Instance Property

# userInterfaceLayoutDirection

The layout direction of the user interface.

macOS 10.8+

``` source
@MainActor
var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection { get set }
```

## Discussion

The default value of this property is NSUserInterfaceLayoutDirection.leftToRight. When the property is set to NSUserInterfaceLayoutDirection.rightToLeft, the table view flips the visual order of the table columns, but the logical order remains unchanged. Although this property was introduced in macOS 10.12, in earlier versions the property always returned NSUserInterfaceLayoutDirection.leftToRight.

## See Also

### Layout Support

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

