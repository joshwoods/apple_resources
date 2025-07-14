

- AppKit
- NSTableViewDiffableDataSourceReference
-  init(tableView:cellProvider:) 

Initializer

# init(tableView:cellProvider:)

Creates a diffable data source with the specified cell provider, and connects it to the specified table view.

macOS 11.0+

``` source
init(
    tableView: NSTableView,
    cellProvider: @escaping NSTableViewDiffableDataSourceReferenceCellProvider
)
```

## Parameters 

`tableView`  

The initialized table view object to connect to the diffable data source.

`cellProvider`  

A closure that creates and returns each of the cells for the table view from the data the diffable data source provides. This replaces the tableView(_:viewFor:row:) delegate method.

## See Also

### Creating a Diffable Data Source

typealias NSTableViewDiffableDataSourceReferenceCellProvider

A closure that configures and returns a cell for a table view from its diffable data source.

