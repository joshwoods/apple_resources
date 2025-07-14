

- UIKit
- UICollectionView
-  prefetchDataSource 

Instance Property

# prefetchDataSource

The object that acts as the prefetching data source for the collection view, receiving notifications of upcoming cell data requirements.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
weak var prefetchDataSource: (any UICollectionViewDataSourcePrefetching)? { get set }
```

## Discussion

Assign an object that conforms to the UICollectionViewDataSourcePrefetching protocol to facilitate prefetching of data for cells to be displayed in the near future. To disable data prefetching behavior, set this property to `nil`.

## See Also

### Prefetching collection view cells and data

var isPrefetchingEnabled: Bool

A Boolean value that indicates whether cell and data prefetching are enabled.

protocol UICollectionViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a collection view, allowing the triggering of asynchronous data load operations.

