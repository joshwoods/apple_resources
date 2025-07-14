

- UIKit
- UISearchDisplayController
-  delegate Deprecated

Instance Property

# delegate

The controller’s delegate.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
unowned(unsafe) var delegate: (any UISearchDisplayDelegate)? { get set }
```

## See Also

### Configuring a search bar

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

var navigationItem: UINavigationItem?

Represents the search display controller in a navigation controller’s navigation bar.

Deprecated

