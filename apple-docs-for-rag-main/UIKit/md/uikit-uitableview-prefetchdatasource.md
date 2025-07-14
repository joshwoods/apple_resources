

- UIKit
- UITableView
-  prefetchDataSource 

Instance Property

# prefetchDataSource

The object that acts as the prefetching data source for the table view, receiving notifications of upcoming cell data requirements.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
weak var prefetchDataSource: (any UITableViewDataSourcePrefetching)? { get set }
```

## Discussion

Assign an object that conforms to the UITableViewDataSourcePrefetching protocol to facilitate prefetching of data for cells to be displayed in the near future. To disable prefetching behavior, set this property to `nil`. This object isn’t retained.

## See Also

### Providing the data and cells

var dataSource: (any UITableViewDataSource)?

The object that acts as the data source of the table view.

var isPrefetchingEnabled: Bool

A Boolean value that indicates whether to allow cell and data prefetching.

protocol UITableViewDataSource

The methods that an object adopts to manage data and provide cells for a table view.

protocol UITableViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a table view, allowing you to start potentially long-running data operations early.

