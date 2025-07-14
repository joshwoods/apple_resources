

- UIKit
- UISearchDisplayController
-  navigationItem Deprecated

Instance Property

# navigationItem

Represents the search display controller in a navigation controller’s navigation bar.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var navigationItem: UINavigationItem? { get }
```

## Discussion

You can configure the navigation item as described in the UINavigationItem, with the exception of configuring the title view.

Important

The system raises an exception if you attempt to set the titleView property for a search display controller’s navigation item.

## See Also

### Configuring a search bar

var delegate: (any UISearchDisplayDelegate)?

The controller’s delegate.

Deprecated

var searchBar: UISearchBar

The search bar.

Deprecated

var searchContentsController: UIViewController

The view controller that manages the contents being searched.

Deprecated

var searchResultsTableView: UITableView

The table view in which the search results are displayed.

Deprecated

var searchResultsDataSource: (any UITableViewDataSource)?

The data source for the table view in which the search results are displayed.

Deprecated

var searchResultsDelegate: (any UITableViewDelegate)?

The delegate for the table view in which the search results are displayed.

Deprecated

var searchResultsTitle: String?

The title for the search results view.

Deprecated

var displaysSearchBarInNavigationBar: Bool

Specifies that the navigation bar contains a search bar.

Deprecated

