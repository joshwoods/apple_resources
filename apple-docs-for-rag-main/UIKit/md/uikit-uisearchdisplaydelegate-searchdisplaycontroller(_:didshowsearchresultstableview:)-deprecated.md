

- UIKit
- UISearchDisplayDelegate
-  searchDisplayController(\_:didShowSearchResultsTableView:) Deprecated

Instance Method

# searchDisplayController(\_:didShowSearchResultsTableView:)

Tells the delegate that the controller just displayed its table view.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func searchDisplayController(
    _ controller: UISearchDisplayController,
    didShowSearchResultsTableView tableView: UITableView
)
```

## Parameters 

`controller`  

The search display controller for which the receiver is the delegate.

`tableView`  

The search display controller’s table view.

## See Also

### Showing and hiding the table view

func searchDisplayController(UISearchDisplayController, willShowSearchResultsTableView: UITableView)

Tells the delegate that the controller is about to display its table view.

Deprecated

func searchDisplayController(UISearchDisplayController, willHideSearchResultsTableView: UITableView)

Tells the delegate that the controller is about to hide its table view.

Deprecated

func searchDisplayController(UISearchDisplayController, didHideSearchResultsTableView: UITableView)

Tells the delegate that the controller just hid its table view.

Deprecated

