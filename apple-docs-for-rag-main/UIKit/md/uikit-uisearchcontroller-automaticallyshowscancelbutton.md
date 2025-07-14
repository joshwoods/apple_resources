

- UIKit
- UISearchController
-  automaticallyShowsCancelButton 

Instance Property

# automaticallyShowsCancelButton

A Boolean indicating whether the search controller manages the visibility of the search bar’s cancel button.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var automaticallyShowsCancelButton: Bool { get set }
```

## Discussion

By default, UISearchController shows the search bar’s cancel button when search becomes active and hides it when the user dismisses search. You can take over responsibility for showing and hiding the cancel button by setting this property to false. If you set the search bar’s showsCancelButton property, this property becomes false.

## See Also

### Configuring the search interface

var obscuresBackgroundDuringPresentation: Bool

A Boolean indicating whether to obscure the underlying content during a search.

var hidesNavigationBarDuringPresentation: Bool

A Boolean indicating whether to hide the navigation bar when searching.

var automaticallyShowsSearchResultsController: Bool

A Boolean indicating whether the search controller manages the visibility of its results controller.

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

