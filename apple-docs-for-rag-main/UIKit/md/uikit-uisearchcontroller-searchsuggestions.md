

- UIKit
- UISearchController
-  searchSuggestions 

Instance Property

# searchSuggestions

A list of suggestions to offer as shortcuts below the search field.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var searchSuggestions: [any UISearchSuggestion]? { get set }
```

## Mentioned in 

Building a desktop-class iPad app

## Discussion

Provide search suggestions to help people complete their query quickly. Update the suggestions as a person types by implementing updateSearchResults(for:).

The presentation of the search suggestions varies according to the platform and searchBarPlacement:

- In tvOS, the suggestions appear in a list below the keyboard.

- In iOS, the suggestions appear in a menu below the search field when the search bar placement is UINavigationItem.SearchBarPlacement.inline, and in a list that overlays the searchResultsController when the search bar placement is UINavigationItem.SearchBarPlacement.stacked. To prevent the search controller from creating and presenting a search suggestions view controller when the searchBarPlacement is UINavigationItem.SearchBarPlacement.stacked, set ignoresSearchSuggestionsForSearchBarPlacementStacked to true when you create the search controller.

When you assign new suggestions to this property, the suggestions onscreen refresh automatically. When a person selects a suggestion, the system sets this property to `nil` and dismisses the search suggestions menu. Implement updateSearchResults(for:selecting:) to execute any necessary updates when a person selects a suggestion.

Note

In tvOS, when a person selects a search suggestion, the search controller automatically updates the search bar’s text according to the value of localizedSuggestion.

If the search suggestions menu dismisses for other reasons, such as a person tapping outside the search bar, searchSuggestions doesn’t reset to `nil` immediately. The system sets searchSuggestions to `nil` only when a person interacts with search directly — for example, by typing in the search field, canceling search, or changing the search scope using the search bar’s scope bar. To dismiss the menu manually, set this property to `nil` or `[]`.

## See Also

### Providing search suggestions

var ignoresSearchSuggestionsForSearchBarPlacementStacked: Bool

A Boolean value you use to specify whether the search controller prevents search suggestions from displaying for a stacked search bar.

class UISearchSuggestionItem

A selectable search parameter.

protocol UISearchSuggestion

A set of attributes that a selectable search suggestion must provide.

