

- UIKit
- UICollectionViewDiffableDataSource
-  UICollectionViewDiffableDataSource.CellProvider 

Type Alias

# UICollectionViewDiffableDataSource.CellProvider

A closure that configures and returns a cell for a collection view from its diffable data source.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
typealias CellProvider = (UICollectionView, IndexPath, ItemIdentifierType) -> UICollectionViewCell?
```

## Parameters 

`collectionView`  

The collection view to configure this cell for.

`indexPath`  

The index path that specifies the location of the cell in the collection view.

`itemIdentifier`  

An object, with a type that implements the Hashable protocol, the data source uses to uniquely identify the item for this cell.

## Return Value

A non-`nil` configured cell object. The cell provider must return a valid cell object to the collection view.

## Discussion

You use this closure to configure and return cells when creating a diffable data source using init(collectionView:cellProvider:).

## See Also

### Related Documentation

class UICollectionViewDiffableDataSourceReference

The object you use to manage data and provide cells for a collection view.

Updating collection views using diffable data sources

Streamline the display and update of data in a collection view using a diffable data source that contains identifiers.

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

### Creating a diffable data source

init(collectionView: UICollectionView, cellProvider: UICollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.CellProvider)

Creates a diffable data source with the specified cell provider, and connects it to the specified collection view.

