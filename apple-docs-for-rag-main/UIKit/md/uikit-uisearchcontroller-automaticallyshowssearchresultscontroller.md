

- UIKit
- UISearchController
-  automaticallyShowsSearchResultsController 

Instance Property

# automaticallyShowsSearchResultsController

A Boolean indicating whether the search controller manages the visibility of its results controller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var automaticallyShowsSearchResultsController: Bool { get set }
```

## Discussion

The default value for this property is true. When it’s true, UISearchController automatically shows its results controller based on the contents of its text property. If you set showsSearchResultsController, this property becomes false.

## See Also

### Configuring the search interface

var obscuresBackgroundDuringPresentation: Bool

A Boolean indicating whether to obscure the underlying content during a search.

var hidesNavigationBarDuringPresentation: Bool

A Boolean indicating whether to hide the navigation bar when searching.

var automaticallyShowsCancelButton: Bool

A Boolean indicating whether the search controller manages the visibility of the search bar’s cancel button.

var showsSearchResultsController: Bool

A Boolean indicating whether the search results controller is visible when the search controller is active.

var searchBarPlacement: UINavigationItem.SearchBarPlacement

The placement of the search bar in the navigation bar.

var ignoresSearchSuggestionsForSearchBarPlacementStacked: Bool

A Boolean value you use to specify whether the search controller prevents search suggestions from displaying for a stacked search bar.

var automaticallyShowsScopeBar: Bool

A Boolean indicating whether the search controller manages the visibility of the search bar’s scope bar.

Deprecated

var scopeBarActivation: UISearchController.ScopeBarActivation

A mode that determines when the search controller shows and hides the scope bar.

enum ScopeBarActivation

Constants that specify the modes for showing and hiding the scope bar.

