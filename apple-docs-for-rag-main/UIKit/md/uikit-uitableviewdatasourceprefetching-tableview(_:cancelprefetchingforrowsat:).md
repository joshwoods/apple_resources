

- UIKit
- UITableViewDataSourcePrefetching
-  tableView(\_:cancelPrefetchingForRowsAt:) 

Instance Method

# tableView(\_:cancelPrefetchingForRowsAt:)

Cancels a previously triggered data prefetch request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    cancelPrefetchingForRowsAt indexPaths: [IndexPath]
)
```

## Parameters 

`tableView`  

The table view issuing the cancellation of the prefetch request.

`indexPaths`  

The index paths of the items for which the data is no longer required.

## Discussion

The table view calls this method on the main queue to cancel prefetch requests for cells that are no longer needed. Use this method to cancel operations initiated by a previous call to tableView(_:prefetchRowsAt:).

For information about how to cancel an asynchronous data loading task, see Concurrency Programming Guide.

## See Also

### Fetching the row data

func tableView(UITableView, prefetchRowsAt: [IndexPath])

Instructs your prefetch data source object to begin preparing data for the cells at the supplied index paths.

**Required**

