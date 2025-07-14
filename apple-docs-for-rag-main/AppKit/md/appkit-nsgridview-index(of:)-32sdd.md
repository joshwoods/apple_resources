

- AppKit
- NSGridView
-  index(of:) 

Instance Method

# index(of:)

Returns the index of the specified grid column.

macOS 10.12+

``` source
@MainActor
func index(of column: NSGridColumn) -> Int
```

## See Also

### Getting Information About the Grid

var numberOfRows: Int

The number of rows in the grid view.

var numberOfColumns: Int

The number of columns in the grid view.

func row(at: Int) -> NSGridRow

Returns the grid row object at the specified index.

func column(at: Int) -> NSGridColumn

Returns the grid column object at the specified index.

func index(of: NSGridRow) -> Int

Returns the index of the specified grid row.

