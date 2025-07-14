

- UIKit
- UICollectionViewDiffableDataSource
- UICollectionViewDiffableDataSource.ReorderingHandlers
-  willReorder 

Instance Property

# willReorder

The handler that prepares the diffable data source for reordering its items.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var willReorder: ((NSDiffableDataSourceTransaction) -> Void)? { get set }
```

## See Also

### Reordering items

var canReorderItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether you can reorder a particular item.

var didReorder: ((NSDiffableDataSourceTransaction&lt;SectionIdentifierType, ItemIdentifierType>) -> Void)?

The handler that processes a reordering transaction.

