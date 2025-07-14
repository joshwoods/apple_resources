

- UIKit
-  UICollectionViewDiffableDataSource 

Class

# UICollectionViewDiffableDataSource

The object you use to manage data and provide cells for a collection view.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
@MainActor @preconcurrency
class UICollectionViewDiffableDataSource where SectionIdentifierType : Hashable, SectionIdentifierType : Sendable, ItemIdentifierType : Hashable, ItemIdentifierType : Sendable
```

## Overview

A *diffable data source* object is a specialized type of data source that works together with your collection view object. It provides the behavior you need to manage updates to your collection view’s data and UI in a simple, efficient way. It also conforms to the UICollectionViewDataSource protocol and provides implementations for all of the protocol’s methods.

To fill a collection view with data:

1.  Connect a diffable data source to your collection view.

2.  Implement a cell provider to configure your collection view’s cells.

3.  Generate the current state of the data.

4.  Display the data in the UI.

To connect a diffable data source to a collection view, you create the diffable data source using its init(collectionView:cellProvider:) initializer, passing in the collection view you want to associate with that data source. You also pass in a cell provider, where you configure each of your cells to determine how to display your data in the UI.

```
dataSource = UICollectionViewDiffableDataSource(collectionView: collectionView) {
    (collectionView: UICollectionView, indexPath: IndexPath, itemIdentifier: UUID) -> UICollectionViewCell? in
    // Configure and return cell.
}
```

Then, you generate the current state of the data and display the data in the UI by constructing and applying a snapshot. For more information, see NSDiffableDataSourceSnapshot.

Important

Don’t change the dataSource on the collection view after you configure it with a diffable data source. If the collection view needs a new data source after you configure it initially, create and configure a new collection view and diffable data source.

## Topics

### Creating a diffable data source

init(collectionView: UICollectionView, cellProvider: UICollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.CellProvider)

Creates a diffable data source with the specified cell provider, and connects it to the specified collection view.

typealias CellProvider

A closure that configures and returns a cell for a collection view from its diffable data source.

### Creating supplementary views

var supplementaryViewProvider: UICollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.SupplementaryViewProvider?

The closure that configures and returns the collection view’s supplementary views, such as headers and footers, from the diffable data source.

typealias SupplementaryViewProvider

A closure that configures and returns a collection view’s supplementary view, such as a header or footer, from a diffable data source.

### Identifying items

func itemIdentifier(for: IndexPath) -> ItemIdentifierType?

Returns an identifier for the item at the specified index path in the collection view.

func indexPath(for: ItemIdentifierType) -> IndexPath?

Returns an index path for the item with the specified identifier in the collection view.

### Identifying sections

func sectionIdentifier(for: Int) -> SectionIdentifierType?

Returns an identifier for the section at the index you specify in the collection view.

func index(for: SectionIdentifierType) -> Int?

Returns an index for the section with the identifier you specify in the collection view.

### Updating data

func snapshot() -> NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>

Returns a representation of the current state of the data in the collection view.

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool) async

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes.

func apply(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the UI to reflect the state of the data in the snapshot, optionally animating the UI changes and executing a completion handler.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>) async

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes.

func applySnapshotUsingReloadData(NSDiffableDataSourceSnapshot&lt;SectionIdentifierType, ItemIdentifierType>, completion: (() -> Void)?)

Resets the UI to reflect the state of the data in the snapshot without computing a diff or animating the changes, optionally executing a completion handler.

### Updating section data

func snapshot(for: SectionIdentifierType) -> NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>

Returns a representation of the current state of the data in the specified section of the collection view.

func apply(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>, to: SectionIdentifierType, animatingDifferences: Bool, completion: (() -> Void)?)

Updates the section UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes and executing a completion handler.

func apply(NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>, to: SectionIdentifierType, animatingDifferences: Bool) async

Updates the section UI to reflect the state of the data in the specified snapshot, optionally animating the UI changes.

### Supporting reordering

var reorderingHandlers: UICollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.ReorderingHandlers

The diffable data source’s handlers for reordering items.

struct ReorderingHandlers

Handlers for reordering items.

struct NSDiffableDataSourceTransaction

A transaction that describes the changes after reordering the items in the view.

struct NSDiffableDataSourceSectionTransaction

A transaction that describes the changes after reordering the items in a section.

### Supporting expanding and collapsing

var sectionSnapshotHandlers: UICollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.SectionSnapshotHandlers&lt;ItemIdentifierType>

The diffable data source’s handlers for expanding and collapsing items.

struct SectionSnapshotHandlers

Handlers for expanding and collapsing items.

### Supporting protocol requirements

Protocol implementations

Access the diffable data source’s implementations of protocol methods.

### Supporting bridging

class UICollectionViewDiffableDataSourceReference

The object you use to manage data and provide cells for a collection view.

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
- UICollectionViewDataSource

## See Also

### Data

Updating collection views using diffable data sources

Streamline the display and update of data in a collection view using a diffable data source that contains identifiers.

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

Building high-performance lists and collection views

Improve the performance of lists and collections in your app with prefetching and image preparation.

protocol UICollectionViewDataSource

The methods adopted by the object you use to manage data and provide cells for a collection view.

protocol UICollectionViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a collection view, allowing the triggering of asynchronous data load operations.

struct NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

struct NSDiffableDataSourceSectionSnapshot

A representation of the state of the data in a layout section at a specific point in time.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

