

- Quartz
- IKImageBrowserView
-  numberOfColumns() 

Instance Method

# numberOfColumns()

Returns the current number of columns.

macOS 10.4+

``` source
@MainActor
func numberOfColumns() -> Int
```

## Return Value

The number of columns.

## See Also

### Getting Columns and Rows Information

func numberOfRows() -> Int

Returns the current number of rows.

func rect(ofColumn: Int) -> NSRect

Returns the rectangle containing the specified column.

func columnIndexes(in: NSRect) -> IndexSet!

Returns the column indexes in the specified rectangle.

func rect(ofRow: Int) -> NSRect

Returns the rectangle containing the specified row.

func rowIndexes(in: NSRect) -> IndexSet!

Returns the row indexes in the specified rectangle.

