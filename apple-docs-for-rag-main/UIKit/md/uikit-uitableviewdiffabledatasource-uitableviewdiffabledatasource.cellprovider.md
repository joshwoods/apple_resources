

- UIKit
- UITableViewDiffableDataSource
-  UITableViewDiffableDataSource.CellProvider 

Type Alias

# UITableViewDiffableDataSource.CellProvider

A closure that configures and returns a cell for a table view from its diffable data source.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
typealias CellProvider = (UITableView, IndexPath, ItemIdentifierType) -> UITableViewCell?
```

## Parameters 

`tableView`  

The table view to configure this cell for.

`indexPath`  

The index path that specifies the location of the cell in the table view.

`itemIdentifier`  

The identifier of the item for this cell.

## Return Value

A non-`nil` configured cell object. The cell provider must return a valid cell object to the table view.

## See Also

### Creating a diffable data source

init(tableView: UITableView, cellProvider: UITableViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.CellProvider)

Creates a diffable data source with the specified cell provider, and connects it to the specified table view.

