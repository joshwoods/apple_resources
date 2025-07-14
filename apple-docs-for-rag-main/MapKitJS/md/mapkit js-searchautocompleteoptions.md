

- MapKit JS
-  SearchAutocompleteOptions 

Structure

# SearchAutocompleteOptions

Options you provide to constrain an autocomplete request.

MapKit JS 5.32.2+

``` source
dictionary SearchAutocompleteOptions {
 string language;
 mapkit.Coordinate coordinate;
 mapkit.CoordinateRegion region;
 string regionPriority;
 boolean includeAddresses;
 boolean includePointsOfInterest;
 boolean includePhysicalFeatures;
 boolean includeQueries;
 mapkit.AddressFilter addressFilter;
 mapkit.PointOfInterestFilter pointOfInterestFilter;
 string limitToCountries;
};
```

## Topics

### Autocomplete search initialization

coordinate

A map coordinate that provides a hint for the geographic area to search.

language

A language ID that determines the language for the search result text.

region

A map region that provides a hint for the geographic area to search.

### Autocomplete search filtering

includePhysicalFeatures

A Boolean value that indicates whether the autocomplete search results include physical features, such as mountain ranges, rivers, and ocean basins.

includePointsOfInterest

A Boolean value that indicates whether the search results include points of interest.

includeQueries

A Boolean value that indicates whether the search results include queries.

limitToCountries

A string that constrains search results to within the provided countries.

regionPriority

A filter that controls whether results occur outside, or strictly within, the region.

### Address filtering

addressFilter

A filter that lists which address options to include or exclude in search results.

includeAddresses

A Boolean value that indicates whether the search results include addresses.

### Points of interest

pointOfInterestFilter

A filter used to include or exclude point of interest categories in search results.

## See Also

### Performing a search autocomplete

autocomplete

Retrieves a list of autocomplete results for the specified search query.

SearchAutocompleteResponse

An object containing the response from an autocomplete request.

SearchAutocompleteResult

The result of an autocomplete query, including display lines and a coordinate.

