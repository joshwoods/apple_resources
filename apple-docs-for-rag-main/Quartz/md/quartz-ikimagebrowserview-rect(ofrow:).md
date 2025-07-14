

- Quartz
- IKImageBrowserView
-  rect(ofRow:) 

Instance Method

# rect(ofRow:)

Returns the rectangle containing the specified row.

macOS 10.4+

``` source
@MainActor
func rect(ofRow rowIndex: Int) -> NSRect
```

## Parameters 

`rowIndex`  

The row index.

## Return Value

A rectangle containing the column. Specified in the view’s coordinate system.

## See Also

### Getting Columns and Rows Information

func numberOfColumns() -> Int

Returns the current number of columns.

func numberOfRows() -> Int

Returns the current number of rows.

func rect(ofColumn: Int) -> NSRect

Returns the rectangle containing the specified column.

func columnIndexes(in: NSRect) -> IndexSet!

Returns the column indexes in the specified rectangle.

func rowIndexes(in: NSRect) -> IndexSet!

Returns the row indexes in the specified rectangle.

