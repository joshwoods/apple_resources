

- UIKit
- UICollectionViewDataSourcePrefetching
-  collectionView(\_:cancelPrefetchingForItemsAt:) 

Instance Method

# collectionView(\_:cancelPrefetchingForItemsAt:)

Cancels a previously triggered data prefetch request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    cancelPrefetchingForItemsAt indexPaths: [IndexPath]
)
```

## Parameters 

`collectionView`  

The collection view issuing the cancellation of the prefetch request.

`indexPaths`  

The index paths that specify the locations of the items for which data is no longer required.

## Discussion

The collection view calls this method to cancel prefetch requests as cells scroll out of view. Your implementation of this method is responsible for canceling the operations initiated by a previous call to collectionView(_:prefetchItemsAt:). For further information about canceling an asynchronous data loading task, see Concurrency Programming Guide.

## See Also

### Managing data prefetching

Prefetching collection view data

Load data for collection view cells before they display.

func collectionView(UICollectionView, prefetchItemsAt: [IndexPath])

Tells your prefetch data source object to begin preparing data for the cells at the supplied index paths.

**Required**

