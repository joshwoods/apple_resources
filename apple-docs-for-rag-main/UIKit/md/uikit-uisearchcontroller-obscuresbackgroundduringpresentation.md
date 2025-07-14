

- UIKit
- UISearchController
-  obscuresBackgroundDuringPresentation 

Instance Property

# obscuresBackgroundDuringPresentation

A Boolean indicating whether to obscure the underlying content during a search.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var obscuresBackgroundDuringPresentation: Bool { get set }
```

## Discussion

When the value of this property is true, the search controller obscures the view controller containing your searchable content as soon as the user interacts with the search bar. When this property is false, the search controller doesn’t obscure the original view controller. This property controls only whether the original view controller is initially obscured. When the user enters text in the search bar, the search controller immediately displays the search results controller with the results.

If you use the same view controller to display the searchable content and search results, it’s recommended that you set this property to false. The default value of this property is true.

## See Also

### Configuring the search interface

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

var automaticallyShowsScopeBar: Bool

A Boolean indicating whether the search controller manages the visibility of the search bar’s scope bar.

Deprecated

var scopeBarActivation: UISearchController.ScopeBarActivation

A mode that determines when the search controller shows and hides the scope bar.

enum ScopeBarActivation

Constants that specify the modes for showing and hiding the scope bar.

