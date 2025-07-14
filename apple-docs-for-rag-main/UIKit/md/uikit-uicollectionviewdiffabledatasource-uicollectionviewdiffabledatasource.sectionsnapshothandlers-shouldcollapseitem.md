

- UIKit
- UICollectionViewDiffableDataSource
- UICollectionViewDiffableDataSource.SectionSnapshotHandlers
-  shouldCollapseItem 

Instance Property

# shouldCollapseItem

The handler that determines whether a particular item is collapsable.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var shouldCollapseItem: ((ItemIdentifierType) -> Bool)? { get set }
```

## See Also

### Expanding and collapsing items

var shouldExpandItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether a particular item is expandable.

var willCollapseItem: ((ItemIdentifierType) -> Void)?

The handler that prepares the diffable data source for collapsing an item.

var willExpandItem: ((ItemIdentifierType) -> Void)?

The handler that prepares the diffable data source for expanding an item.

var snapshotForExpandingParent: ((ItemIdentifierType, NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>) -> NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>)?

The handler that provides the section snapshot for expanding the parent item.

