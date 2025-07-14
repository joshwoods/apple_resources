

- UIKit
- UITableView
-  dataSource 

Instance Property

# dataSource

The object that acts as the data source of the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var dataSource: (any UITableViewDataSource)? { get set }
```

## Discussion

The data source must adopt the UITableViewDataSource protocol. The data source isn’t retained.

## See Also

### Related Documentation

var delegate: (any UITableViewDelegate)?

The object that acts as the delegate of the table view.

### Providing the data and cells

var prefetchDataSource: (any UITableViewDataSourcePrefetching)?

The object that acts as the prefetching data source for the table view, receiving notifications of upcoming cell data requirements.

var isPrefetchingEnabled: Bool

A Boolean value that indicates whether to allow cell and data prefetching.

protocol UITableViewDataSource

The methods that an object adopts to manage data and provide cells for a table view.

protocol UITableViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a table view, allowing you to start potentially long-running data operations early.

