

- AppKit
- NSCollectionViewDiffableDataSource
-  init(collectionView:itemProvider:) 

Initializer

# init(collectionView:itemProvider:)

Creates a diffable data source with the specified item provider, and connects it to the specified collection view.

macOS 10.15.1+

``` source
init(
    collectionView: NSCollectionView,
    itemProvider: @escaping NSCollectionViewDiffableDataSource.ItemProvider
)
```

## Parameters 

`collectionView`  

The initialized collection view object to connect to the diffable data source.

`itemProvider`  

A closure that creates and returns each of the items for the collection view from the data the diffable data source provides.

## See Also

### Creating a Diffable Data Source

typealias ItemProvider

A closure that configures and returns an item for a collection view from its diffable data source.

