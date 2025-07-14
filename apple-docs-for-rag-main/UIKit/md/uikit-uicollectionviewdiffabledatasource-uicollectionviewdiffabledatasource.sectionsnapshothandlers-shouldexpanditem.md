

- UIKit
- UICollectionViewDiffableDataSource
- UICollectionViewDiffableDataSource.SectionSnapshotHandlers
-  shouldExpandItem 

Instance Property

# shouldExpandItem

The handler that determines whether a particular item is expandable.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
var shouldExpandItem: ((ItemIdentifierType) -> Bool)? { get set }
```

## See Also

### Expanding and collapsing items

var shouldCollapseItem: ((ItemIdentifierType) -> Bool)?

The handler that determines whether a particular item is collapsable.

var willCollapseItem: ((ItemIdentifierType) -> Void)?

The handler that prepares the diffable data source for collapsing an item.

var willExpandItem: ((ItemIdentifierType) -> Void)?

The handler that prepares the diffable data source for expanding an item.

var snapshotForExpandingParent: ((ItemIdentifierType, NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>) -> NSDiffableDataSourceSectionSnapshot&lt;ItemIdentifierType>)?

The handler that provides the section snapshot for expanding the parent item.

