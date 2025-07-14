

- AppKit
- NSTableView
-  noteNumberOfRowsChanged() 

Instance Method

# noteNumberOfRowsChanged()

Informs the table view that the number of records in its data source has changed.

macOS

``` source
@MainActor
func noteNumberOfRowsChanged()
```

## Discussion

This method allows the table view to update the scrollers in its scroll view without actually reloading data into the table view. It’s useful for a data source that continually receives data in the background over a period of time, in which case the table view can remain responsive to the user while the data is received.

See the NSTableViewDataSource protocol specification for information on the messages an `NSTableView` object sends to its data source.

Note

When using NSView-based table views this method should be avoided. The table will query the data source for the new number of rows, and properly insert (or remove) rows at the end of the table as necessary with an animation.

When using NSCell-based table views this method tells the table that there may be more (or less) rows available and to reload state based on that information.

This method does not work for NSOutlineView, and should not be called.

## See Also

### Related Documentation

func reloadData()

Marks the table view as needing redisplay, so it will reload the data for visible cells and draw the new values.

func numberOfRows(in: NSTableView) -> Int

Returns the number of records managed for `aTableView` by the data source object.

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

func frameOfCell(atColumn: Int, row: Int) -> NSRect

Returns a rectangle locating the cell that lies at the intersection of the specified column and row.

var columnAutoresizingStyle: NSTableView.ColumnAutoresizingStyle

The table view’s column autoresizing style.

func sizeLastColumnToFit()

Resizes the last column so the table view fits exactly within its enclosing clip view.

func tile()

Properly sizes the table view and its header view and marks it as needing display.

func sizeToFit()

Sizes the table view based on a uniform column autoresizing style.

func noteHeightOfRows(withIndexesChanged: IndexSet)

Informs the table view that the rows specified in `indexSet` have changed height.

