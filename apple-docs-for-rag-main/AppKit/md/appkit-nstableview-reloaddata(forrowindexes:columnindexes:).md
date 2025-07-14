

- AppKit
- NSTableView
-  reloadData(forRowIndexes:columnIndexes:) 

Instance Method

# reloadData(forRowIndexes:columnIndexes:)

Reloads the data for only the specified rows and columns.

macOS 10.6+

``` source
@MainActor
func reloadData(
    forRowIndexes rowIndexes: IndexSet,
    columnIndexes: IndexSet
)
```

## Parameters 

`rowIndexes`  

The indexes of the rows to update.

`columnIndexes`  

The indexes of the columns to update.

## Discussion

For cells that are visible, the appropriate dataSource and delegate methods are called and the cells are redrawn.

For tables that support variable row heights, the row height is not re-queried from the delegate; it is your responsibility to invoke noteHeightOfRows(withIndexesChanged:) if a row height change is required.

Note

For NSView-based table views, this method drops the view-cells in the table row, but not the NSTableRowView instances.

## See Also

### Managing the Table’s Data

var dataSource: (any NSTableViewDataSource)?

The object that provides the data displayed by the table view.

var usesStaticContents: Bool

A Boolean value indicating whether the table uses static data.

func reloadData()

Marks the table view as needing redisplay, so it will reload the data for visible cells and draw the new values.

