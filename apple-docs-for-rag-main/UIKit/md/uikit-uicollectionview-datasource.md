

- UIKit
- UICollectionView
-  dataSource 

Instance Property

# dataSource

The object that provides the data for the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var dataSource: (any UICollectionViewDataSource)? { get set }
```

## Discussion

The data source must adopt the UICollectionViewDataSource protocol. The collection view maintains a weak reference to the data source object.

## See Also

### Providing the collection view data

class UICollectionViewDiffableDataSource

The object you use to manage data and provide cells for a collection view.

protocol UICollectionViewDataSource

The methods adopted by the object you use to manage data and provide cells for a collection view.

Building high-performance lists and collection views

Improve the performance of lists and collections in your app with prefetching and image preparation.

