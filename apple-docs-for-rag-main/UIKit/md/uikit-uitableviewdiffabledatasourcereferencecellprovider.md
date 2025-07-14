

- UIKit
-  UITableViewDiffableDataSourceReferenceCellProvider 

Type Alias

# UITableViewDiffableDataSourceReferenceCellProvider

A closure that configures and returns a cell for a table view from its diffable data source.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
typealias UITableViewDiffableDataSourceReferenceCellProvider = (UITableView, IndexPath, Any) -> UITableViewCell?
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

init(tableView: UITableView, cellProvider: UITableViewDiffableDataSourceReferenceCellProvider)

Creates a diffable data source with the specified cell provider, and connects it to the specified table view.

