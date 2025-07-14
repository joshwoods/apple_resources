

- UIKit
- UICollectionViewDiffableDataSource
- UICollectionViewDiffableDataSource.ReorderingHandlers
-  canReorderItem 

Instance Property

# canReorderItem

The handler that determines whether you can reorder a particular item.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var canReorderItem: ((ItemIdentifierType) -> Bool)? { get set }
```

## See Also

### Reordering items

var willReorder: ((NSDiffableDataSourceTransaction&lt;SectionIdentifierType, ItemIdentifierType>) -> Void)?

The handler that prepares the diffable data source for reordering its items.

var didReorder: ((NSDiffableDataSourceTransaction&lt;SectionIdentifierType, ItemIdentifierType>) -> Void)?

The handler that processes a reordering transaction.

