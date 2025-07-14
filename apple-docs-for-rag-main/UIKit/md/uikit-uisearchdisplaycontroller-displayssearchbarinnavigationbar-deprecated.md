

- UIKit
- UISearchDisplayController
-  displaysSearchBarInNavigationBar Deprecated

Instance Property

# displaysSearchBarInNavigationBar

Specifies that the navigation bar contains a search bar.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var displaysSearchBarInNavigationBar: Bool { get set }
```

## Discussion

When you return true to display the search bar in a navigation bar, the system uses the search display controller’s navigationItem property and ignores the navigation item, if set, of the searchContentsController view controller. The displayed search field occupies as much width in the navigation bar as possible.

A search bar displayed in a navigation bar cannot have a scope bar.

Important

The system raises an exception if you set the showsScopeBar property to true in a search bar that is displayed in a navigation bar.

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

var navigationItem: UINavigationItem?

Represents the search display controller in a navigation controller’s navigation bar.

Deprecated

