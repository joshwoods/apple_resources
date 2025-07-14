

- UIKit
- UISearchController
-  searchBarPlacement 

Instance Property

# searchBarPlacement

The placement of the search bar in the navigation bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var searchBarPlacement: UINavigationItem.SearchBarPlacement { get }
```

## Discussion

This placement applies only when the search controller is associated with a navigation item through its searchController property.

## See Also

### Configuring the search interface

var obscuresBackgroundDuringPresentation: Bool

A Boolean indicating whether to obscure the underlying content during a search.

var hidesNavigationBarDuringPresentation: Bool

A Boolean indicating whether to hide the navigation bar when searching.

var automaticallyShowsCancelButton: Bool

A Boolean indicating whether the search controller manages the visibility of the search bar’s cancel button.

var automaticallyShowsSearchResultsController: Bool

A Boolean indicating whether the search controller manages the visibility of its results controller.

var showsSearchResultsController: Bool

A Boolean indicating whether the search results controller is visible when the search controller is active.

var ignoresSearchSuggestionsForSearchBarPlacementStacked: Bool

A Boolean value you use to specify whether the search controller prevents search suggestions from displaying for a stacked search bar.

var automaticallyShowsScopeBar: Bool

A Boolean indicating whether the search controller manages the visibility of the search bar’s scope bar.

Deprecated

var scopeBarActivation: UISearchController.ScopeBarActivation

A mode that determines when the search controller shows and hides the scope bar.

enum ScopeBarActivation

Constants that specify the modes for showing and hiding the scope bar.

