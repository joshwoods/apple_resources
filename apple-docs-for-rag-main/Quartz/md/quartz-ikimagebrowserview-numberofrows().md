

- Quartz
- IKImageBrowserView
-  numberOfRows() 

Instance Method

# numberOfRows()

Returns the current number of rows.

macOS 10.4+

``` source
@MainActor
func numberOfRows() -> Int
```

## Return Value

The number of rows.

## See Also

### Getting Columns and Rows Information

func numberOfColumns() -> Int

Returns the current number of columns.

func rect(ofColumn: Int) -> NSRect

Returns the rectangle containing the specified column.

func columnIndexes(in: NSRect) -> IndexSet!

Returns the column indexes in the specified rectangle.

func rect(ofRow: Int) -> NSRect

Returns the rectangle containing the specified row.

func rowIndexes(in: NSRect) -> IndexSet!

Returns the row indexes in the specified rectangle.

