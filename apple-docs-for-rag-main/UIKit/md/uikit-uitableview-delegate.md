

- UIKit
- UITableView
-  delegate 

Instance Property

# delegate

The object that acts as the delegate of the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UITableViewDelegate)? { get set }
```

## Discussion

The delegate must adopt the UITableViewDelegate protocol. The delegate isn’t retained.

## See Also

### Related Documentation

var dataSource: (any UITableViewDataSource)?

The object that acts as the data source of the table view.

### Managing interactions with the table

protocol UITableViewDelegate

Methods for managing selections, configuring section headers and footers, deleting and reordering cells, and performing other actions in a table view.

