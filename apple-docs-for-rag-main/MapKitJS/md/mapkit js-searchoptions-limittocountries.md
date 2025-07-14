

- MapKit JS
- SearchOptions
-  limitToCountries 

Instance Property

# limitToCountries

A string that constrains search results to within the provided countries.

MapKit JS 5.49+

``` source
attribute string limitToCountries;
```

## Discussion

The string is a comma-separated list of two-digit ISO 3166-2 country and region codes. For example, to limit search results to Germany, Belgium, and France specify `de,be,fr`.

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

pointOfInterestFilter

A filter for including or excluding point-of-interest categories in search results.

region

A map region that provides a hint for the geographic area to search.

regionPriority

A filter that controls whether results occur outside, or strictly within, the region.

