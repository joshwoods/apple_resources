

- AppKit
-  NSTableViewDiffableDataSourceReferenceRowProvider 

Type Alias

# NSTableViewDiffableDataSourceReferenceRowProvider

A closure that configures and returns a row view for a table view from its diffable data source.

macOS

``` source
typealias NSTableViewDiffableDataSourceReferenceRowProvider = (NSTableView, Int, Any) -> NSTableRowView
```

## See Also

### Creating Row and Section Views

var rowViewProvider: NSTableViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.RowProvider?

The closure that configures and returns the table view’s row views from the diffable data source.

var sectionHeaderViewProvider: NSTableViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.SectionHeaderViewProvider?

The closure that configures and returns the table view’s section header views from the diffable data source.

typealias RowProvider

A closure that configures and returns a row view for a table view from its diffable data source.

typealias SectionHeaderViewProvider

A closure that configures and returns a section header view for a table view from its diffable data source.

typealias NSTableViewDiffableDataSourceReferenceSectionHeaderViewProvider

A closure that configures and returns a section header view for a table view from its diffable data source.

