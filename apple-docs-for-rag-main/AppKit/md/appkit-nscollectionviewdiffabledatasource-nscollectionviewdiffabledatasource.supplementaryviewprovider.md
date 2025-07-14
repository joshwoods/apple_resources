

- AppKit
- NSCollectionViewDiffableDataSource
-  NSCollectionViewDiffableDataSource.SupplementaryViewProvider 

Type Alias

# NSCollectionViewDiffableDataSource.SupplementaryViewProvider

A closure that configures and returns a collection view’s supplementary view, such as a header or footer, from a diffable data source.

macOS 10.15.1+

``` source
typealias SupplementaryViewProvider = (NSCollectionView, String, IndexPath) -> (any NSView & NSCollectionViewElement)?
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

### Creating Supplementary Views

var supplementaryViewProvider: NSCollectionViewDiffableDataSource&lt;SectionIdentifierType, ItemIdentifierType>.SupplementaryViewProvider?

The closure that configures and returns the collection view’s supplementary views, such as headers and footers, from the diffable data source.

