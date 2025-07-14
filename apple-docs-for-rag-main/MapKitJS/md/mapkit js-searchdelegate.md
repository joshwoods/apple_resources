

- MapKit JS
-  SearchDelegate 

Class

# SearchDelegate

An object or callback function the framework calls when performing a search or an autocomplete request.

MapKit JS 5.0+

``` source
interface SearchDelegate
```

## Overview

You can also pass an object to the search and autocomplete methods instead of a search delegate callback function. A delegate object can include the following methods:

- searchDidComplete. Upon successful completion of a search request, this method returns a data object that’s the same as the one that passes to the search callback function.

- searchDidError. The system calls this when the search request fails.

- autocompleteDidComplete. When an autocomplete request successfully completes, this method returns a `data` array that’s the same as the one that passes to the autocomplete callback function.

- autocompleteDidError. The system invokes this when an autocomplete request fails.

## Topics

### Responding to state changes and errors

autocompleteDidComplete

Tells the delegate when the autocomplete request completes.

autocompleteDidError

Tells the delegate when the autocomplete request fails due to an error.

searchDidComplete

Tells the delegate when the search completes.

searchDidError

Tells the delegate when the search fails due to an error.

## See Also

### Performing a search

search

Retrieves the results of a search query.

SearchOptions

An object that contains options to adjust a search.

SearchResponse

The result of a search, including the original search query, the bounding region, and a list of places that match the query.

