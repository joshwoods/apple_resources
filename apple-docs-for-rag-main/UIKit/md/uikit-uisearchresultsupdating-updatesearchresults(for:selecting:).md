

- UIKit
- UISearchResultsUpdating
-  updateSearchResults(for:selecting:) 

Instance Method

# updateSearchResults(for:selecting:)

Asks the object to update the search results for a specified controller after the user selects a search suggestion.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
optional func updateSearchResults(
    for searchController: UISearchController,
    selecting searchSuggestion: any UISearchSuggestion
)
```

## Parameters 

`searchController`  

The UISearchController object used as the search bar.

`searchSuggestion`  

The suggestion the user selected.

## Discussion

The system calls this method when the user selects a search suggestion. Perform any required filtering and updating of search results or suggestions inside of this method.

## See Also

### Updating the search bar

func updateSearchResults(for: UISearchController)

Asks the object to update the search results for a specified controller.

**Required**

