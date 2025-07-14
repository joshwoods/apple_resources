

- UIKit
-  UITableViewDataSourcePrefetching 

Protocol

# UITableViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a table view, allowing you to start potentially long-running data operations early.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITableViewDataSourcePrefetching : NSObjectProtocol
```

## Mentioned in 

Filling a table with data

## Overview

You use a prefetch data source object in conjunction with your table view’s data source to begin loading data for cells before the tableView(_:cellForRowAt:) data source method is called. The following steps are required to support a prefetch data source to your table view:

- Create the table view and its regular data source.

- Create an object that adopts the UITableViewDataSourcePrefetching protocol, and assign it to the prefetchDataSource property on the table view.

- Initiate asynchronous loading of the data required for the cells at the specified index paths in your implementation of tableView(_:prefetchRowsAt:).

- Prepare the cell for display using the prefetched data in your tableView(_:cellForRowAt:) data source method.

- Cancel pending data load operations when the table view informs you that the data is no longer required in the tableView(_:cancelPrefetchingForRowsAt:) method.

Note

The prefetch method isn’t necessarily called for every cell in the table view. For details about a suggested approach to loading data, see Load data asynchronously.

When configuring the table view object, assign your prefetch data source to its prefetchDataSource property. For more information about how a table view works, see UITableView.

### Load data asynchronously

The tableView(_:prefetchRowsAt:) method isn’t necessarily called for every cell in the table view. Your implementation of tableView(_:cellForRowAt:) must therefore be able to cope with the following potential situations:

- Data has been loaded via the prefetch request, and is ready to be displayed.

- Data is currently being prefetched, but isn’t yet available.

- Data hasn’t yet been requested.

One approach that handles all of these situations is to use Operation to load the data for each row. You create the Operation object and store it in the prefetch method. The data source method can then either retrieve the operation and the result, or create it if it doesn’t exist. For further information about how you can use asynchronous programming models to achieve this desired behavior, see Concurrency Programming Guide.

## Topics

### Fetching the row data

func tableView(UITableView, prefetchRowsAt: [IndexPath])

Instructs your prefetch data source object to begin preparing data for the cells at the supplied index paths.

**Required**

func tableView(UITableView, cancelPrefetchingForRowsAt: [IndexPath])

Cancels a previously triggered data prefetch request.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Data

Filling a table with data

Create and configure cells for your table dynamically using a data source object, or provide them statically from your storyboard.

Asynchronously loading images into table and collection views

Store and fetch images asynchronously to make your app more responsive.

protocol UITableViewDataSource

The methods that an object adopts to manage data and provide cells for a table view.

class UITableViewDiffableDataSource

The object you use to manage data and provide cells for a table view.

struct NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

class UILocalizedIndexedCollation

An object that organizes, sorts, and localizes the data for a table view that has a section index.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

