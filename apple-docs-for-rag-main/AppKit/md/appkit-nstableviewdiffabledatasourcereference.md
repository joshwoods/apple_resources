

- AppKit
-  NSTableViewDiffableDataSourceReference 

Class

# NSTableViewDiffableDataSourceReference

The object you use to manage data and provide items for a table view.

macOS 11.0+

``` source
class NSTableViewDiffableDataSourceReference where SectionIdentifierType : AnyObject, ItemIdentifierType : AnyObject
```

## Overview

Important

If you’re working in a Swift codebase, always use NSTableViewDiffableDataSource instead of `NSTableViewDiffableDataSourceReference`.

A *diffable data source* object is a specialized type of data source that works together with your table view object. It provides the behavior you need to manage updates to your table view’s data and UI in a simple, efficient way. It also conforms to the NSTableViewDataSource protocol.

To fill a table view with data:

1.  Connect a diffable data source to your table view.

2.  Implement a cell provider to configure your table view’s cells.

3.  Generate the current state of the data.

4.  Display the data in the UI.

To connect a diffable data source to a table view, you create the diffable data source using its init(tableView:cellProvider:) initializer, passing in the table view you want to associate with that data source. You also pass in a cell provider, where you configure each of your cells to determine how to display your data in the UI.

Then, you generate the current state of the data and display the data in the UI by constructing and applying a snapshot. For more information, see NSDiffableDataSourceSnapshotReference.

## Topics

### Creating a Diffable Data Source

init(tableView: NSTableView, cellProvider: NSTableViewDiffableDataSourceReferenceCellProvider)

Creates a diffable data source with the specified cell provider, and connects it to the specified table view.

typealias NSTableViewDiffableDataSourceReferenceCellProvider

A closure that configures and returns a cell for a table view from its diffable data source.

### Creating Row and Section Views

var rowViewProvider: NSTableViewDiffableDataSourceReferenceRowProvider?

The closure that configures and returns the table view’s row views from the diffable data source.

var sectionHeaderViewProvider: NSTableViewDiffableDataSourceReferenceSectionHeaderViewProvider?

The closure that configures and returns the table view’s section header views from the diffable data source.

typealias NSTableViewDiffableDataSourceReferenceRowProvider

A closure that configures and returns a row view for a table view from its diffable data source.

typealias NSTableViewDiffableDataSourceReferenceSectionHeaderViewProvider

A closure that configures and returns a section header view for a table view from its diffable data source.

### Identifying Items and Sections

func itemIdentifier(forRow: Int) -> ItemIdentifierType?

Returns an identifier for the item at the specified row in the table view.

func row(forItemIdentifier: ItemIdentifierType) -> Int

Returns a row for the item with the specified identifier in the table view.

func sectionIdentifier(forRow: Int) -> SectionIdentifierType?

Returns the identifier of the section containing the specified row in the snapshot.

func row(forSectionIdentifier: SectionIdentifierType) -> Int

Returns a row for the section with the specified identifier in the table view.

### Updating Data

func snapshot() -> NSDiffableDataSourceSnapshotReference

Returns a representation of the current state of the data in the table view.

func applySnapshot(NSDiffableDataSourceSnapshotReference, animatingDifferences: Bool)

Updates the UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes.

func applySnapshot(NSDiffableDataSourceSnapshotReference, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes and executing a completion handler.

var defaultRowAnimation: NSTableView.AnimationOptions

The default animation the UI uses to show differences between rows.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- NSTableViewDataSource

