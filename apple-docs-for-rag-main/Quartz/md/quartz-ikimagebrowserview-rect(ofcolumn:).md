

- Quartz
- IKImageBrowserView
-  rect(ofColumn:) 

Instance Method

# rect(ofColumn:)

Returns the rectangle containing the specified column.

macOS 10.4+

``` source
@MainActor
func rect(ofColumn columnIndex: Int) -> NSRect
```

## Parameters 

`columnIndex`  

The column index.

## Return Value

A rectangle containing the column. Specified in the view’s coordinate system.

## See Also

### Getting Columns and Rows Information

func numberOfColumns() -> Int

Returns the current number of columns.

func numberOfRows() -> Int

Returns the current number of rows.

func columnIndexes(in: NSRect) -> IndexSet!

Returns the column indexes in the specified rectangle.

func rect(ofRow: Int) -> NSRect

Returns the rectangle containing the specified row.

func rowIndexes(in: NSRect) -> IndexSet!

Returns the row indexes in the specified rectangle.

