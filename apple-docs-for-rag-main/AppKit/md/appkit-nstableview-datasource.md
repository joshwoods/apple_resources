

- AppKit
- NSTableView
-  dataSource 

Instance Property

# dataSource

The object that provides the data displayed by the table view.

macOS

``` source
@MainActor
weak var dataSource: (any NSTableViewDataSource)? { get set }
```

## Discussion

The data source for the table view must implement the appropriate methods of the NSTableViewDataSource protocol. See Populating a Table View Programmatically and the NSTableViewDataSource `protocol` specification for more information. Note that in versions of macOS prior to v10.12, the table view did not retain the data source in a managed memory environment.

Setting the data source invokes tile().

If the delegate doesn’t respond to either numberOfRows(in:) or tableView(_:objectValueFor:row:), internalInconsistencyException may be raised.

## See Also

### Managing the Table’s Data

var usesStaticContents: Bool

A Boolean value indicating whether the table uses static data.

func reloadData()

Marks the table view as needing redisplay, so it will reload the data for visible cells and draw the new values.

func reloadData(forRowIndexes: IndexSet, columnIndexes: IndexSet)

Reloads the data for only the specified rows and columns.

