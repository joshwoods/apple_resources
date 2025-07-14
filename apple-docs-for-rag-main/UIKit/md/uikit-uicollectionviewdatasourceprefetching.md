

- UIKit
-  UICollectionViewDataSourcePrefetching 

Protocol

# UICollectionViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a collection view, allowing the triggering of asynchronous data load operations.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UICollectionViewDataSourcePrefetching : NSObjectProtocol
```

## Overview

You use a prefetch data source object in conjunction with your collection view’s data source to begin loading data for cells before the collectionView(_:cellForItemAt:) data source method is called.

Follow these steps to add a prefetch data source to your collection view:

1.  Create the collection view and its data source.

2.  Create an object that adopts the UICollectionViewDataSourcePrefetching protocol, and assign it to the prefetchDataSource property on the collection view.

3.  Initiate asynchronous loading of the data required for the cells at the specified index paths in your implementation of collectionView(_:prefetchItemsAt:).

4.  Prepare the cell for display using the prefetched data in your implementation of the collectionView(_:cellForItemAt:) data source method.

5.  Cancel pending data load operations when the collection view informs you that the data is no longer required in the collectionView(_:cancelPrefetchingForItemsAt:) method.

Note

The prefetch method isn’t necessarily called for every cell in the collection view. See Load data asynchronously for details on a suggested approach to loading data.

For more information, see UICollectionView.

### Load data asynchronously

The collectionView(_:prefetchItemsAt:) method isn’t necessarily called for every cell in the collection view. Your implementation of collectionView(_:cellForItemAt:) must therefore be able to cope with the following potential situations:

- Data has been loaded via the prefetch request, and is ready to be displayed.

- Data is currently being prefetched, but isn’t yet available.

- Data hasn’t yet been requested.

One approach that handles all of these situations is to use Operation to load the data for each row. You create the Operation object and store it in the prefetch method. The data source method can then either retrieve the operation and the result, or create it if it doesn’t exist. For further information about how you can use asynchronous programming models to achieve this desired behavior, see Concurrency Programming Guide.

## Topics

### Managing data prefetching

Prefetching collection view data

Load data for collection view cells before they display.

func collectionView(UICollectionView, prefetchItemsAt: [IndexPath])

Tells your prefetch data source object to begin preparing data for the cells at the supplied index paths.

**Required**

func collectionView(UICollectionView, cancelPrefetchingForItemsAt: [IndexPath])

Cancels a previously triggered data prefetch request.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Data

Updating collection views using diffable data sources

Streamline the display and update of data in a collection view using a diffable data source that contains identifiers.

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

Building high-performance lists and collection views

Improve the performance of lists and collections in your app with prefetching and image preparation.

class UICollectionViewDiffableDataSource

The object you use to manage data and provide cells for a collection view.

protocol UICollectionViewDataSource

The methods adopted by the object you use to manage data and provide cells for a collection view.

struct NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

struct NSDiffableDataSourceSectionSnapshot

A representation of the state of the data in a layout section at a specific point in time.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

