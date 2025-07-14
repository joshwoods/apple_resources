

- MapKit JS
-  SearchConstructorOptions 

Structure

# SearchConstructorOptions

Options you provide when you create a search object.

MapKit JS 5.0+

``` source
dictionary SearchConstructorOptions {
 string language;
 boolean getsUserLocation;
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

### Search Initialization

coordinate

A map coordinate that provides a hint for the geographic area to search.

getsUserLocation

A Boolean value that indicates whether to limit the search results to the user’s location, according to the web browser.

language

A language ID that determines the language for the search results text.

region

A map region that provides a hint for the geographic area to search.

### Search filtering

includePhysicalFeatures

A Boolean value that indicates whether the search results include physical features, such as mountain ranges, rivers, and ocean basins.

includeQueries

A Boolean value that indicates whether the search results include queries.

limitToCountries

A string that constrains search results to within the provided countries.

regionPriority

A filter that controls whether results occur outside, or strictly within, the region.

### Address filtering

addressFilter

A filter that lists which address components to include or exclude in search results.

includeAddresses

A Boolean value that indicates whether the search results include addresses.

### Points of Interest

includePointsOfInterest

A Boolean value that indicates whether the search results should include points of interest.

pointOfInterestFilter

A filter used to include or exclude point of interest categories.

## See Also

### Creating a search

mapkit.Search

Creates a search object with optional initial values that you provide.

