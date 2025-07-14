

- MapKit JS
-  mapkit.Search 

Class

# mapkit.Search

An object that retrieves map-based search results for a user-entered query.

MapKit JS 5.0+

``` source
interface mapkit.Search
```

## Overview

The search service allows developers to populate a map with results from a user-entered query, including information about businesses and other points of interest. MapKit JS provides this functionality through a search object that makes network requests to the search service.

Supplying *search context* creates the most relevant results for a query. Context may include the user’s location, or a coordinate or region that the developer provides.

To use the search service, create an instance of a search object with the desired options. Use the search object to make search requests.

## Topics

### Creating a search

mapkit.Search

Creates a search object with optional initial values that you provide.

SearchConstructorOptions

Options you provide when you create a search object.

### Performing a search

search

Retrieves the results of a search query.

SearchDelegate

An object or callback function the framework calls when performing a search or an autocomplete request.

SearchOptions

An object that contains options to adjust a search.

SearchResponse

The result of a search, including the original search query, the bounding region, and a list of places that match the query.

### Performing a search autocomplete

autocomplete

Retrieves a list of autocomplete results for the specified search query.

SearchAutocompleteOptions

Options you provide to constrain an autocomplete request.

SearchAutocompleteResponse

An object containing the response from an autocomplete request.

SearchAutocompleteResult

The result of an autocomplete query, including display lines and a coordinate.

### Filtering a search

mapkit.AddressCategory

The categories of address components that users can search for with an address filter.

mapkit.AddressFilter

An object that filters which address options to include or exclude in search results.

mapkit.Search.RegionPriority

A value that indicates the importance of the configured region.

### Canceling a search

cancel

Cancels a search request using its request ID.

## See Also

### Search

mapkit.AddressCategory

The categories of address components that users can search for with an address filter.

mapkit.AddressFilter

An object that filters which address options to include or exclude in search results.

