

- UIKit
- UISearchController
-  automaticallyShowsScopeBar Deprecated

Instance Property

# automaticallyShowsScopeBar

A Boolean indicating whether the search controller manages the visibility of the search bar’s scope bar.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.1+tvOS 13.0+visionOS 1.0–2.4Deprecated

``` source
@MainActor
var automaticallyShowsScopeBar: Bool { get set }
```

Deprecated

In iOS, use scopeBarActivation instead.

## Discussion

By default, UISearchController shows the search bar’s scope bar when search becomes active and hides it when the user dismisses the search. Set this to false if you want to show and hide the scope bar in your own code. If you set the showsScopeBar property, that also changes this property to false.

Note

The search bar doesn’t show its scope bar at all if there are fewer than two titles in the search bar’s scopeButtonTitles.

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

var ignoresSearchSuggestionsForSearchBarPlacementStacked: Bool

A Boolean value you use to specify whether the search controller prevents search suggestions from displaying for a stacked search bar.

var scopeBarActivation: UISearchController.ScopeBarActivation

A mode that determines when the search controller shows and hides the scope bar.

enum ScopeBarActivation

Constants that specify the modes for showing and hiding the scope bar.

