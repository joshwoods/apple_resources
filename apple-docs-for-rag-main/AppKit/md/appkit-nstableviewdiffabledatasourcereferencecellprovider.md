

- AppKit
-  NSTableViewDiffableDataSourceReferenceCellProvider 

Type Alias

# NSTableViewDiffableDataSourceReferenceCellProvider

A closure that configures and returns a cell for a table view from its diffable data source.

macOS

``` source
typealias NSTableViewDiffableDataSourceReferenceCellProvider = (NSTableView, NSTableColumn, Int, Any) -> NSView
```

## See Also

### Creating a Diffable Data Source

init(tableView: NSTableView, cellProvider: NSTableViewDiffableDataSourceReferenceCellProvider)

Creates a diffable data source with the specified cell provider, and connects it to the specified table view.

