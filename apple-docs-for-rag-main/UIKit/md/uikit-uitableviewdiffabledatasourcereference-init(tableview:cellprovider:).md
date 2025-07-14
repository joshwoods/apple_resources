

- UIKit
- UITableViewDiffableDataSourceReference
-  init(tableView:cellProvider:) 

Initializer

# init(tableView:cellProvider:)

Creates a diffable data source with the specified cell provider, and connects it to the specified table view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(
    tableView: UITableView,
    cellProvider: @escaping UITableViewDiffableDataSourceReferenceCellProvider
)
```

## Parameters 

`tableView`  

The initialized table view object to connect to the diffable data source.

`cellProvider`  

A closure that creates and returns each of the cells for the table view from the data the diffable data source provides.

## See Also

### Creating a diffable data source

typealias UITableViewDiffableDataSourceReferenceCellProvider

A closure that configures and returns a cell for a table view from its diffable data source.

