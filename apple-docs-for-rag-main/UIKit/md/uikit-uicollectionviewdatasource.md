

- UIKit
-  UICollectionViewDataSource 

Protocol

# UICollectionViewDataSource

The methods adopted by the object you use to manage data and provide cells for a collection view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UICollectionViewDataSource : NSObjectProtocol
```

## Overview

A data source object manages the data in your collection view. It represents your app’s data model and vends information to the collection view as needed. It also creates and configures the cells and supplementary views that the collection view uses to display your data.

A collection view data source must conform to the UICollectionViewDataSource protocol. You can use a UICollectionViewDiffableDataSource object as your data source object, which already conforms to this protocol.

Alternatively, you can create a custom data source object by adopting the UICollectionViewDataSource protocol. At a minimum, all data source objects must implement the collectionView(_:numberOfItemsInSection:) and collectionView(_:cellForItemAt:) methods. These methods are responsible for returning the number of items in the collection view along with the items themselves. The remaining methods of the protocol are optional and only needed if your collection view organizes items into multiple sections or provides headers and footers for a given section.

When you configure the collection view object, assign your data source to its dataSource property. For more information about how a collection view works with its data source to present content, see UICollectionView.

## Topics

### Getting item and section metrics

func collectionView(UICollectionView, numberOfItemsInSection: Int) -> Int

Asks your data source object for the number of items in the specified section.

**Required**

func numberOfSections(in: UICollectionView) -> Int

Asks your data source object for the number of sections in the collection view.

### Getting views for items

func collectionView(UICollectionView, cellForItemAt: IndexPath) -> UICollectionViewCell

Asks your data source object for the cell that corresponds to the specified item in the collection view.

**Required**

func collectionView(UICollectionView, viewForSupplementaryElementOfKind: String, at: IndexPath) -> UICollectionReusableView

Asks your data source object to provide a supplementary view to display in the collection view.

### Reordering items

func collectionView(UICollectionView, canMoveItemAt: IndexPath) -> Bool

Asks your data source object whether the specified item can move to another location in the collection view.

func collectionView(UICollectionView, moveItemAt: IndexPath, to: IndexPath)

Tells your data source object to move the specified item to its new location.

### Configuring an index

func indexTitles(for: UICollectionView) -> [String]?

Asks the data source to return the titles for the index items to display for the collection view.

func collectionView(UICollectionView, indexPathForIndexTitle: String, at: Int) -> IndexPath

Asks the data source to return the index path of a collection view item that corresponds to one of your index entries.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UICollectionViewController
- UICollectionViewDiffableDataSource
- UICollectionViewDiffableDataSourceReference

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

protocol UICollectionViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a collection view, allowing the triggering of asynchronous data load operations.

struct NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

struct NSDiffableDataSourceSectionSnapshot

A representation of the state of the data in a layout section at a specific point in time.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

