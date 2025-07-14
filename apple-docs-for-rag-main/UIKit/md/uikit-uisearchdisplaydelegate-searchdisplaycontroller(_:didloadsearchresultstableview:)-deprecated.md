

- UIKit
- UISearchDisplayDelegate
-  searchDisplayController(\_:didLoadSearchResultsTableView:) Deprecated

Instance Method

# searchDisplayController(\_:didLoadSearchResultsTableView:)

Tells the delegate that the controller has loaded its table view.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func searchDisplayController(
    _ controller: UISearchDisplayController,
    didLoadSearchResultsTableView tableView: UITableView
)
```

## Parameters 

`controller`  

The search display controller for which the receiver is the delegate.

`tableView`  

The search display controller’s table view.

## See Also

### Loading and unloading the table view

func searchDisplayController(UISearchDisplayController, willUnloadSearchResultsTableView: UITableView)

Tells the delegate that the controller is about to unload its table view.

Deprecated

