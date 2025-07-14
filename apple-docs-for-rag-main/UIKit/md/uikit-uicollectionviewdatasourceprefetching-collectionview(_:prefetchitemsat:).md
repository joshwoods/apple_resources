

- UIKit
- UICollectionViewDataSourcePrefetching
-  collectionView(\_:prefetchItemsAt:) 

Instance Method

# collectionView(\_:prefetchItemsAt:)

Tells your prefetch data source object to begin preparing data for the cells at the supplied index paths.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func collectionView(
    _ collectionView: UICollectionView,
    prefetchItemsAt indexPaths: [IndexPath]
)
```

**Required**

## Parameters 

`collectionView`  

The collection view issuing the prefetch request.

`indexPaths`  

The index paths that specify the locations of the items for which the data is to be prefetched.

## Discussion

The collection view calls this method as the user scrolls, providing the index paths for cells it’s likely to display in the near future. Your implementation of this method is responsible for starting any expensive data loading processes. The data loading must be performed asynchronously, and the results made available to the collectionView(_:cellForItemAt:) method on the collection view’s data source.

The collection view doesn’t call this method for cells it requires immediately, so your code must not rely on this method to load data. The order of the index paths provided represents the priority.

For further information about creating an asynchronous data loading task, see Concurrency Programming Guide.

## See Also

### Managing data prefetching

Prefetching collection view data

Load data for collection view cells before they display.

func collectionView(UICollectionView, cancelPrefetchingForItemsAt: [IndexPath])

Cancels a previously triggered data prefetch request.

