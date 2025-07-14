

- UIKit
-  UISearchResultsUpdating 

Protocol

# UISearchResultsUpdating

A set of methods that let you update search results based on information the user enters into the search bar.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UISearchResultsUpdating : NSObjectProtocol
```

## Topics

### Updating the search bar

func updateSearchResults(for: UISearchController)

Asks the object to update the search results for a specified controller.

**Required**

func updateSearchResults(for: UISearchController, selecting: any UISearchSuggestion)

Asks the object to update the search results for a specified controller after the user selects a search suggestion.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Search interface

class UISearchContainerViewController

A view controller that manages the presentation of search results in your interface.

class UISearchController

A view controller that manages the display of search results based on interactions with a search bar.

class UISearchBar

A specialized view for receiving search-related information from the user.

Displaying searchable content by using a search controller

Create a user interface with searchable content in a table view.

Using suggested searches with a search controller

Create a search interface with a table view of suggested searches.

