

- Quartz
- IKImageBrowserView
-  rowIndexes(in:) 

Instance Method

# rowIndexes(in:)

Returns the row indexes in the specified rectangle.

macOS 10.4+

``` source
@MainActor
func rowIndexes(in rect: NSRect) -> IndexSet!
```

## Parameters 

`rect`  

A rectangle in the view’s coordinate system.

## Return Value

An index set containing the item indexes.

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

func rect(ofRow: Int) -> NSRect

Returns the rectangle containing the specified row.

