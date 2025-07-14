

- AppKit
- NSTableViewDiffableDataSource
-  NSTableViewDiffableDataSource.CellProvider 

Type Alias

# NSTableViewDiffableDataSource.CellProvider

A closure that configures and returns a cell for a table view from its diffable data source.

macOS 11.0+

``` source
typealias CellProvider = (NSTableView, NSTableColumn, Int, ItemIdentifierType) -> NSView
```

## See Also

### Creating a Diffable Data Source

init(tableView: NSTableView, cellProvider: NSTableViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.CellProvider)

Creates a diffable data source with the specified cell provider, and connects it to the specified table view.

