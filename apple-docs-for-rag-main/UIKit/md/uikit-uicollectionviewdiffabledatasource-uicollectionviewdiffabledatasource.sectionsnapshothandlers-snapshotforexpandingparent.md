

- UIKit
- UICollectionViewDiffableDataSource
- UICollectionViewDiffableDataSource.SectionSnapshotHandlers
-  snapshotForExpandingParent 

Instance Property

# snapshotForExpandingParent

The handler that provides the section snapshot for expanding the parent item.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var snapshotForExpandingParent: ((ItemIdentifierType, NSDiffableDataSourceSectionSnapshot) -> NSDiffableDataSourceSectionSnapshot)? { get set }
```

## Discussion

Use the snapshotForExpandingParent handler to customize the snapshot that returns when a particular parent item is expanded.

```
// Allow every item to be collapsed
dataSource.sectionSnapshotHandlers.shouldCollapseItem = { item in return true }

dataSource.sectionSnapshotHandlers.snapshotForExpandingParent = {
    parent, existingSnapshot -> NSDiffableDataSourceSectionSnapshot in

    // Return child snapshot for the parent, or just existingSnapshot
}
```

## See Also

### Expanding and collapsing items

var shouldCollapseItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether a particular item is collapsable.

var shouldExpandItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether a particular item is expandable.

var willCollapseItem: ((ItemIdentifierType) -> Void)?

The handler that prepares the diffable data source for collapsing an item.

var willExpandItem: ((ItemIdentifierType) -> Void)?

The handler that prepares the diffable data source for expanding an item.

