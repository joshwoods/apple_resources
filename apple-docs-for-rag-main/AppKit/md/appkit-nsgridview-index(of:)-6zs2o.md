

- AppKit
- NSGridView
-  index(of:) 

Instance Method

# index(of:)

Returns the index of the specified grid row.

macOS 10.12+

``` source
@MainActor
func index(of row: NSGridRow) -> Int
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

func column(at: Int) -> NSGridColumn

Returns the grid column object at the specified index.

