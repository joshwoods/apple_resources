

- UIKit
- UISearchDisplayDelegate
-  searchDisplayController(\_:willUnloadSearchResultsTableView:) Deprecated

Instance Method

# searchDisplayController(\_:willUnloadSearchResultsTableView:)

Tells the delegate that the controller is about to unload its table view.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func searchDisplayController(
    _ controller: UISearchDisplayController,
    willUnloadSearchResultsTableView tableView: UITableView
)
```

## Parameters 

`controller`  

The search display controller for which the receiver is the delegate.

`tableView`  

The search display controller’s table view.

## See Also

### Loading and unloading the table view

func searchDisplayController(UISearchDisplayController, didLoadSearchResultsTableView: UITableView)

Tells the delegate that the controller has loaded its table view.

Deprecated

