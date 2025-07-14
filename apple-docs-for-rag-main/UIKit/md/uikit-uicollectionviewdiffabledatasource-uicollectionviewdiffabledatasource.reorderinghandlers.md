

- UIKit
- UICollectionViewDiffableDataSource
-  UICollectionViewDiffableDataSource.ReorderingHandlers 

Structure

# UICollectionViewDiffableDataSource.ReorderingHandlers

Handlers for reordering items.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct ReorderingHandlers
```

Available when `SectionIdentifierType` conforms to `Hashable`, `SectionIdentifierType` conforms to `Sendable`, `ItemIdentifierType` conforms to `Hashable`, and `ItemIdentifierType` conforms to `Sendable`.

## Topics

### Reordering items

var canReorderItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether you can reorder a particular item.

var willReorder: ((NSDiffableDataSourceTransaction&lt;SectionIdentifierType, ItemIdentifierType>) -> Void)?

The handler that prepares the diffable data source for reordering its items.

var didReorder: ((NSDiffableDataSourceTransaction&lt;SectionIdentifierType, ItemIdentifierType>) -> Void)?

The handler that processes a reordering transaction.

### Initializers

init()

Creates a reordering handlers structure.

## See Also

### Supporting reordering

var reorderingHandlers: UICollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.ReorderingHandlers

The diffable data source’s handlers for reordering items.

struct NSDiffableDataSourceTransaction

A transaction that describes the changes after reordering the items in the view.

struct NSDiffableDataSourceSectionTransaction

A transaction that describes the changes after reordering the items in a section.

