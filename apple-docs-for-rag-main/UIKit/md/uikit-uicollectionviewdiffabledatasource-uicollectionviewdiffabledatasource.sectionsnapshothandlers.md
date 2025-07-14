

- UIKit
- UICollectionViewDiffableDataSource
-  UICollectionViewDiffableDataSource.SectionSnapshotHandlers 

Structure

# UICollectionViewDiffableDataSource.SectionSnapshotHandlers

Handlers for expanding and collapsing items.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@preconcurrency
struct SectionSnapshotHandlers where ItemIdentifierType : Hashable, ItemIdentifierType : Sendable
```

Available when `SectionIdentifierType` conforms to `Hashable`, `SectionIdentifierType` conforms to `Sendable`, `ItemIdentifierType` conforms to `Hashable`, and `ItemIdentifierType` conforms to `Sendable`.

## Topics

### Expanding and collapsing items

var shouldCollapseItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether a particular item is collapsable.

var shouldExpandItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether a particular item is expandable.

var willCollapseItem: ((ItemIdentifierType) -> Void)?

The handler that prepares the diffable data source for collapsing an item.

var willExpandItem: ((ItemIdentifierType) -> Void)?

The handler that prepares the diffable data source for expanding an item.

var snapshotForExpandingParent: ((ItemIdentifierType, NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>) -> NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>)?

The handler that provides the section snapshot for expanding the parent item.

### Initializers

init()

Creates a section snapshot handlers structure.

## See Also

### Supporting expanding and collapsing

var sectionSnapshotHandlers: UICollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.SectionSnapshotHandlers&lt;ItemIdentifierType>

The diffable data source’s handlers for expanding and collapsing items.

