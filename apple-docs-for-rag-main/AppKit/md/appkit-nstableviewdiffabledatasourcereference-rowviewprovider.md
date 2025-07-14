

- AppKit
- NSTableViewDiffableDataSourceReference
-  rowViewProvider 

Instance Property

# rowViewProvider

The closure that configures and returns the table view’s row views from the diffable data source.

macOS 11.0+

``` source
var rowViewProvider: NSTableViewDiffableDataSourceReferenceRowProvider? { get set }
```

## Discussion

This property replaces the tableView(_:rowViewForRow:) delegate method.

## See Also

### Creating Row and Section Views

var sectionHeaderViewProvider: NSTableViewDiffableDataSourceReferenceSectionHeaderViewProvider?

The closure that configures and returns the table view’s section header views from the diffable data source.

typealias NSTableViewDiffableDataSourceReferenceRowProvider

A closure that configures and returns a row view for a table view from its diffable data source.

typealias NSTableViewDiffableDataSourceReferenceSectionHeaderViewProvider

A closure that configures and returns a section header view for a table view from its diffable data source.

