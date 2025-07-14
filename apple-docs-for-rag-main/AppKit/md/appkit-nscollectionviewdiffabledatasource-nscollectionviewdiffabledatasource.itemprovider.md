

- AppKit
- NSCollectionViewDiffableDataSource
-  NSCollectionViewDiffableDataSource.ItemProvider 

Type Alias

# NSCollectionViewDiffableDataSource.ItemProvider

A closure that configures and returns an item for a collection view from its diffable data source.

macOS 10.15.1+

``` source
typealias ItemProvider = (NSCollectionView, IndexPath, ItemIdentifierType) -> NSCollectionViewItem?
```

## Parameters 

`collectionView`  

The collection view to configure this item for.

`indexPath`  

The index path that specifies the location of the item in the collection view.

`itemIdentifier`  

The identifier of the data item for this item.

## Return Value

A non-`nil` configured item object. The item provider must return a valid item object to the collection view.

## See Also

### Creating a Diffable Data Source

init(collectionView: NSCollectionView, itemProvider: NSCollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.ItemProvider)

Creates a diffable data source with the specified item provider, and connects it to the specified collection view.

