

- UIKit
- UISearchController
-  ignoresSearchSuggestionsForSearchBarPlacementStacked 

Instance Property

# ignoresSearchSuggestionsForSearchBarPlacementStacked

A Boolean value you use to specify whether the search controller prevents search suggestions from displaying for a stacked search bar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var ignoresSearchSuggestionsForSearchBarPlacementStacked: Bool { get set }
```

## Discussion

Defaults to false. To prevent the search controller from creating and presenting a search suggestions view controller when the searchBarPlacement is UINavigationItem.SearchBarPlacement.stacked, set to true when you create the search controller.

If you set this value to true after the search controller has already displayed search suggestions, it hides the search suggestions view controller and won’t display it again until you set the value to false.

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

var searchBarPlacement: UINavigationItem.SearchBarPlacement

The placement of the search bar in the navigation bar.

var automaticallyShowsScopeBar: Bool

A Boolean indicating whether the search controller manages the visibility of the search bar’s scope bar.

Deprecated

var scopeBarActivation: UISearchController.ScopeBarActivation

A mode that determines when the search controller shows and hides the scope bar.

enum ScopeBarActivation

Constants that specify the modes for showing and hiding the scope bar.

