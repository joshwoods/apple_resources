

- MapKit JS
-  SearchResponse 

Structure

# SearchResponse

The result of a search, including the original search query, the bounding region, and a list of places that match the query.

MapKit JS 5.0+

``` source
dictionary SearchResponse {
 string query;
 mapkit.CoordinateRegion boundingRegion;
 Place[] places;
};
```

## Mentioned in 

MapKit JS 5

## Overview

The search callback function provides the search response in its data parameter. An object parsed from server-returned JSON, `data` contains a query and a boundingRegion.

## Topics

### Search response

places

A list of places that match the search query.

query

The query string for performing the search.

boundingRegion

The region that encloses the places from the search results.

## See Also

### Performing a search

search

Retrieves the results of a search query.

SearchDelegate

An object or callback function the framework calls when performing a search or an autocomplete request.

SearchOptions

An object that contains options to adjust a search.

