

- MapKit JS
-  SearchOptions 

Structure

# SearchOptions

An object that contains options to adjust a search.

MapKit JS 5.0+

``` source
dictionary SearchOptions {
 string language;
 mapkit.Coordinate coordinate;
 mapkit.CoordinateRegion region;
 string regionPriority;
 boolean includeAddresses;
 boolean includePointsOfInterest;
 boolean includePhysicalFeatures;
 mapkit.AddressFilter addressFilter;
 mapkit.PointOfInterestFilter pointOfInterestFilter;
 string limitToCountries;
};
```

## Topics

### Search options

addressFilter

An object that filters which address components to include or exclude in search results.

coordinate

A map coordinate that provides a hint for the geographic area to search.

includeAddresses

A Boolean value that indicates whether the search results should include addresses.

includePhysicalFeatures

A Boolean value that indicates whether the search results include physical features, such as mountain ranges, rivers, and ocean basins.

includePointsOfInterest

A Boolean value that indicates whether the search results should include points of interest.

language

A language ID that determines the language for the search result text.

limitToCountries

A string that constrains search results to within the provided countries.

pointOfInterestFilter

A filter for including or excluding point-of-interest categories in search results.

region

A map region that provides a hint for the geographic area to search.

regionPriority

A filter that controls whether results occur outside, or strictly within, the region.

## See Also

### Performing a search

search

Retrieves the results of a search query.

SearchDelegate

An object or callback function the framework calls when performing a search or an autocomplete request.

SearchResponse

The result of a search, including the original search query, the bounding region, and a list of places that match the query.

