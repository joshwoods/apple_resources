

- UIKit
- UICollectionViewDiffableDataSource
-  reorderingHandlers 

Instance Property

# reorderingHandlers

The diffable data source’s handlers for reordering items.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
var reorderingHandlers: UICollectionViewDiffableDataSource.ReorderingHandlers { get set }
```

Available when `SectionIdentifierType` conforms to `Hashable`, `SectionIdentifierType` conforms to `Sendable`, `ItemIdentifierType` conforms to `Hashable`, and `ItemIdentifierType` conforms to `Sendable`.

## Discussion

Provide reordering handlers to support the reordering of items in your collection view.

The system calls the didReorder handler after a reordering transaction (NSDiffableDataSourceTransaction) occurs, so you can update your data backing store with information about the changes.

```
// Allow every item to be reordered
dataSource.reorderingHandlers.canReorderItem = { item in return true }

// Option 1: Update the backing store from a CollectionDifference
dataSource.reorderingHandlers.didReorder = { [weak self] transaction in
    guard let self = self else { return }

    if let updatedBackingStore = self.backingStore.applying(transaction.difference) {
        self.backingStore = updatedBackingStore
    }
}

// Option 2: Update the backing store from the final item identifiers
dataSource.reorderingHandlers.didReorder = { [weak self] transaction in
    guard let self = self else { return }

    self.backingStore = transaction.finalSnapshot.itemIdentifiers
}
```

## See Also

### Supporting reordering

struct ReorderingHandlers

Handlers for reordering items.

struct NSDiffableDataSourceTransaction

A transaction that describes the changes after reordering the items in the view.

struct NSDiffableDataSourceSectionTransaction

A transaction that describes the changes after reordering the items in a section.

