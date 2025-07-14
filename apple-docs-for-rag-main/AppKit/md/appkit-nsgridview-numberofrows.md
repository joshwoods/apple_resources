

- AppKit
- NSGridView
-  numberOfRows 

Instance Property

# numberOfRows

The number of rows in the grid view.

macOS 10.12+

``` source
@MainActor
var numberOfRows: Int { get }
```

## See Also

### Getting Information About the Grid

var numberOfColumns: Int

The number of columns in the grid view.

func index(of: NSGridColumn) -> Int

Returns the index of the specified grid column.

func row(at: Int) -> NSGridRow

Returns the grid row object at the specified index.

func column(at: Int) -> NSGridColumn

Returns the grid column object at the specified index.

func index(of: NSGridRow) -> Int

Returns the index of the specified grid row.

