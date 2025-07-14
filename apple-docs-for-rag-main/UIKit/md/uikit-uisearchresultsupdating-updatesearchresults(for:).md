

- UIKit
- UISearchResultsUpdating
-  updateSearchResults(for:) 

Instance Method

# updateSearchResults(for:)

Asks the object to update the search results for a specified controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func updateSearchResults(for searchController: UISearchController)
```

**Required**

## Parameters 

`searchController`  

The UISearchController object used as the search bar.

## Discussion

The system calls this method when the search bar becomes the first responder or the search bar’s text changes. Perform any required filtering and updating of search results or suggestions inside of this method.

## See Also

### Updating the search bar

func updateSearchResults(for: UISearchController, selecting: any UISearchSuggestion)

Asks the object to update the search results for a specified controller after the user selects a search suggestion.

