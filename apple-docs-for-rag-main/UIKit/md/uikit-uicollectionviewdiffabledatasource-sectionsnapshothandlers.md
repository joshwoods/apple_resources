

- UIKit
- UICollectionViewDiffableDataSource
-  sectionSnapshotHandlers 

Instance Property

# sectionSnapshotHandlers

The diffable data source’s handlers for expanding and collapsing items.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
var sectionSnapshotHandlers: UICollectionViewDiffableDataSource.SectionSnapshotHandlers { get set }
```

Available when `SectionIdentifierType` conforms to `Hashable`, `SectionIdentifierType` conforms to `Sendable`, `ItemIdentifierType` conforms to `Hashable`, and `ItemIdentifierType` conforms to `Sendable`.

## Discussion

Provide section snapshot handlers to support the expanding or collapsing of items in your collection view.

Use the snapshotForExpandingParent handler to customize the snapshot that returns when a particular parent item is expanded.

```
// Allow every item to be collapsed
dataSource.sectionSnapshotHandlers.shouldCollapseItem = { item in return true }

dataSource.sectionSnapshotHandlers.snapshotForExpandingParent = {
    parent, currentChildSnapshot -> NSDiffableDataSourceSectionSnapshot in

    // Return child snapshot for the parent, or just currentChildSnapshot
}
```

## See Also

### Supporting expanding and collapsing

struct SectionSnapshotHandlers

Handlers for expanding and collapsing items.

