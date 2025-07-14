

- UIKit
- UISearchDisplayController
-  searchResultsTitle Deprecated

Instance Property

# searchResultsTitle

The title for the search results view.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var searchResultsTitle: String? { get set }
```

## Discussion

The default value is `nil`.

If the value is `nil`, the controller uses the default title string.

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

var displaysSearchBarInNavigationBar: Bool

Specifies that the navigation bar contains a search bar.

Deprecated

var navigationItem: UINavigationItem?

Represents the search display controller in a navigation controller’s navigation bar.

Deprecated

