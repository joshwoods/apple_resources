

- AppKit
- NSGridView
-  column(at:) 

Instance Method

# column(at:)

Returns the grid column object at the specified index.

macOS 10.12+

``` source
@MainActor
func column(at index: Int) -> NSGridColumn
```

## See Also

### Getting Information About the Grid

var numberOfRows: Int

The number of rows in the grid view.

var numberOfColumns: Int

The number of columns in the grid view.

func index(of: NSGridColumn) -> Int

Returns the index of the specified grid column.

func row(at: Int) -> NSGridRow

Returns the grid row object at the specified index.

func index(of: NSGridRow) -> Int

Returns the index of the specified grid row.

