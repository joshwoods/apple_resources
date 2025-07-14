

- UIKit
- UICollectionViewDiffableDataSource
- UICollectionViewDiffableDataSource.SectionSnapshotHandlers
-  willExpandItem 

Instance Property

# willExpandItem

The handler that prepares the diffable data source for expanding an item.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var willExpandItem: ((ItemIdentifierType) -> Void)? { get set }
```

## See Also

### Expanding and collapsing items

var shouldCollapseItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether a particular item is collapsable.

var shouldExpandItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether a particular item is expandable.

var willCollapseItem: ((ItemIdentifierType) -> Void)?

The handler that prepares the diffable data source for collapsing an item.

var snapshotForExpandingParent: ((ItemIdentifierType, NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>) -> NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>)?

The handler that provides the section snapshot for expanding the parent item.

