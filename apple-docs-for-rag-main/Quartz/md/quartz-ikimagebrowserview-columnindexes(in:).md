

- Quartz
- IKImageBrowserView
-  columnIndexes(in:) 

Instance Method

# columnIndexes(in:)

Returns the column indexes in the specified rectangle.

macOS 10.4+

``` source
@MainActor
func columnIndexes(in rect: NSRect) -> IndexSet!
```

## Parameters 

`rect`  

The rectangle in the view’s coordinate system.

## Return Value

An index set containing the cell indexes.

## See Also

### Getting Columns and Rows Information

func numberOfColumns() -> Int

Returns the current number of columns.

func numberOfRows() -> Int

Returns the current number of rows.

func rect(ofColumn: Int) -> NSRect

Returns the rectangle containing the specified column.

func rect(ofRow: Int) -> NSRect

Returns the rectangle containing the specified row.

func rowIndexes(in: NSRect) -> IndexSet!

Returns the row indexes in the specified rectangle.

