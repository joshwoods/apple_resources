

- UIKit
- UICollectionViewDiffableDataSource
-  UICollectionViewDiffableDataSource.SupplementaryViewProvider 

Type Alias

# UICollectionViewDiffableDataSource.SupplementaryViewProvider

A closure that configures and returns a collection view’s supplementary view, such as a header or footer, from a diffable data source.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
typealias SupplementaryViewProvider = (UICollectionView, String, IndexPath) -> UICollectionReusableView?
```

## Parameters 

`collectionView`  

The collection view to configure this supplementary view for.

`kind`  

The kind of supplementary view to provide. The layout object that supports the supplementary view defines the value of this string.

`indexPath`  

The index path that specifies the location of the supplementary view in the collection view.

## Return Value

A non-`nil` configured supplementary view object. The supplementary view provider must return a valid view object to the collection view.

## See Also

### Creating supplementary views

var supplementaryViewProvider: UICollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.SupplementaryViewProvider?

The closure that configures and returns the collection view’s supplementary views, such as headers and footers, from the diffable data source.

