

- MapKit JS
- SearchOptions
-  region 

Instance Property

# region

A map region that provides a hint for the geographic area to search.

MapKit JS 5.0+

``` source
attribute mapkit.CoordinateRegion region;
```

## Discussion

This overrides the region provided to the mapkit.Search constructor.

## See Also

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

regionPriority

A filter that controls whether results occur outside, or strictly within, the region.

