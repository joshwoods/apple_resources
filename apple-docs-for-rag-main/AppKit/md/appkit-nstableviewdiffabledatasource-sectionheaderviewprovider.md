

- AppKit
- NSTableViewDiffableDataSource
-  sectionHeaderViewProvider 

Instance Property

# sectionHeaderViewProvider

The closure that configures and returns the table view’s section header views from the diffable data source.

macOS 11.0+

``` source
var sectionHeaderViewProvider: NSTableViewDiffableDataSource.SectionHeaderViewProvider?
```

## Discussion

This property replaces the tableView(_:viewFor:row:) method for group rows when the `tableColumn` parameter in tableView(_:viewFor:row:) would be `nil`. Setting this property means the table view never invokes its delegate’s tableView(_:isGroupRow:) method. Instead, it uses the current snapshot’s sections.

## See Also

### Creating Row and Section Views

var rowViewProvider: NSTableViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.RowProvider?

The closure that configures and returns the table view’s row views from the diffable data source.

typealias RowProvider

A closure that configures and returns a row view for a table view from its diffable data source.

typealias NSTableViewDiffableDataSourceReferenceRowProvider

A closure that configures and returns a row view for a table view from its diffable data source.

typealias SectionHeaderViewProvider

A closure that configures and returns a section header view for a table view from its diffable data source.

typealias NSTableViewDiffableDataSourceReferenceSectionHeaderViewProvider

A closure that configures and returns a section header view for a table view from its diffable data source.

