

- UIKit
- UISearchController
-  searchResultsUpdater 

Instance Property

# searchResultsUpdater

The object responsible for updating the contents of the search results controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var searchResultsUpdater: (any UISearchResultsUpdating)? { get set }
```

## Discussion

Assign an object that adopts the UISearchResultsUpdating protocol. Use the methods of that protocol to search your content and deliver the results to your search results view controller. The object contained by the searchResultsUpdater property is often the view controller that’s set during initialization.

## See Also

### Managing the search results

var searchBar: UISearchBar

The search bar to install in your interface.

var searchResultsController: UIViewController?

The view controller that displays the results of the search.

var isActive: Bool

The presented state of the search interface.

