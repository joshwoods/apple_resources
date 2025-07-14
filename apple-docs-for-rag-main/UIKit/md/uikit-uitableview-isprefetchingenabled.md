

- UIKit
- UITableView
-  isPrefetchingEnabled 

Instance Property

# isPrefetchingEnabled

A Boolean value that indicates whether to allow cell and data prefetching.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var isPrefetchingEnabled: Bool { get set }
```

## Discussion

When true, the table view may request cells in advance of displaying them. When false, the table view requests cells when they need to display. Setting this property to false also disables data prefetching. The default value of this property is true.

## See Also

### Providing the data and cells

var dataSource: (any UITableViewDataSource)?

The object that acts as the data source of the table view.

var prefetchDataSource: (any UITableViewDataSourcePrefetching)?

The object that acts as the prefetching data source for the table view, receiving notifications of upcoming cell data requirements.

protocol UITableViewDataSource

The methods that an object adopts to manage data and provide cells for a table view.

protocol UITableViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a table view, allowing you to start potentially long-running data operations early.

