

- MapKit JS
- SearchOptions
-  regionPriority 

Instance Property

# regionPriority

A filter that controls whether results occur outside, or strictly within, the region.

MapKit JS 5.78.1+

``` source
attribute string regionPriority;
```

## Discussion

Use this property to filter places that exist outside the bounds of a region that may have the same name.

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

region

A map region that provides a hint for the geographic area to search.

