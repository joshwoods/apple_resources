

- UIKit
- UISearchController
-  isActive 

Instance Property

# isActive

The presented state of the search interface.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isActive: Bool { get set }
```

## Discussion

When the user taps in the search field of a managed search bar, the search controller automatically displays the search results controller. Usually, you get the value of this property to determine whether the search results are displayed. However, you can set this property to true to force the search interface to appear, even if the user hasn’t tapped in the search field.

The default value of this property is false.

## See Also

### Managing the search results

var searchBar: UISearchBar

The search bar to install in your interface.

var searchResultsUpdater: (any UISearchResultsUpdating)?

The object responsible for updating the contents of the search results controller.

var searchResultsController: UIViewController?

The view controller that displays the results of the search.

