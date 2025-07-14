

- UIKit
-  UITableViewDiffableDataSource 

Class

# UITableViewDiffableDataSource

The object you use to manage data and provide cells for a table view.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
@MainActor @preconcurrency
class UITableViewDiffableDataSource where SectionIdentifierType : Hashable, SectionIdentifierType : Sendable, ItemIdentifierType : Hashable, ItemIdentifierType : Sendable
```

## Overview

A *diffable data source* object is a specialized type of data source that works together with your table view object. It provides the behavior you need to manage updates to your table view’s data and UI in a simple, efficient way. It also conforms to the UITableViewDataSource protocol and provides implementations for all of the protocol’s methods.

To fill a table view with data:

1.  Connect a diffable data source to your table view.

2.  Implement a cell provider to configure your table view’s cells.

3.  Generate the current state of the data.

4.  Display the data in the UI.

To connect a diffable data source to a table view, you create the diffable data source using its init(tableView:cellProvider:) initializer, passing in the table view you want to associate with that data source. You also pass in a cell provider, where you configure each of your cells to determine how to display your data in the UI.

```
dataSource = UITableViewDiffableDataSource(tableView: tableView) {
    (tableView: UITableView, indexPath: IndexPath, itemIdentifier: UUID) -> UITableViewCell? in
    // configure and return cell
}
```

Then, you generate the current state of the data and display the data in the UI by constructing and applying a snapshot. For more information, see NSDiffableDataSourceSnapshot.

Important

Do not change the dataSource on the table view after you configure it with a diffable data source. If the table view needs a new data source after you configure it initially, create and configure a new table view and diffable data source.

## Topics

### Creating a diffable data source

init(tableView: UITableView, cellProvider: UITableViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.CellProvider)

Creates a diffable data source with the specified cell provider, and connects it to the specified table view.

typealias CellProvider

A closure that configures and returns a cell for a table view from its diffable data source.

### Identifying items

func itemIdentifier(for: IndexPath) -> ItemIdentifierType?

Returns an identifier for the item at the specified index path in the table view.

func indexPath(for: ItemIdentifierType) -> IndexPath?

Returns an index path for the item with the specified identifier in the table view.

### Identifying sections

func sectionIdentifier(for: Int) -> SectionIdentifierType?

Returns an identifier for the section at the index you specify in the table view.

func index(for: SectionIdentifierType) -> Int?

Returns an index for the section with the identifier you specify in the table view.

### Updating data

func snapshot() -> NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

Returns a representation of the current state of the data in the table view.

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool) async

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes.

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes and executing a completion handler.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>) async

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, completion: (() -> Void)?)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes, optionally executing a completion handler.

var defaultRowAnimation: UITableView.RowAnimation

The default type of animation to use when inserting or deleting rows.

### Supporting bridging

class UITableViewDiffableDataSourceReference

The object you use to manage data and provide cells for a table view.

### Supporting protocol requirements

Protocol implementations

Access the diffable data source’s implementations of protocol methods.

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
- Sendable
- UITableViewDataSource

## See Also

### Data

Filling a table with data

Create and configure cells for your table dynamically using a data source object, or provide them statically from your storyboard.

Asynchronously loading images into table and collection views

Store and fetch images asynchronously to make your app more responsive.

protocol UITableViewDataSource

The methods that an object adopts to manage data and provide cells for a table view.

protocol UITableViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a table view, allowing you to start potentially long-running data operations early.

struct NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

class UILocalizedIndexedCollation

An object that organizes, sorts, and localizes the data for a table view that has a section index.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

