

- UIKit
- UICollectionViewDiffableDataSource
- UICollectionViewDiffableDataSource.ReorderingHandlers
-  didReorder 

Instance Property

# didReorder

The handler that processes a reordering transaction.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var didReorder: ((NSDiffableDataSourceTransaction) -> Void)? { get set }
```

## Discussion

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

### Reordering items

var canReorderItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether you can reorder a particular item.

var willReorder: ((NSDiffableDataSourceTransaction&lt;SectionIdentifierType, ItemIdentifierType>) -> Void)?

The handler that prepares the diffable data source for reordering its items.

