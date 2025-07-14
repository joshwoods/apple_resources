

- MapKit JS
- SearchConstructorOptions
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

### Search filtering

includePhysicalFeatures

A Boolean value that indicates whether the search results include physical features, such as mountain ranges, rivers, and ocean basins.

includeQueries

A Boolean value that indicates whether the search results include queries.

regionPriority

A filter that controls whether results occur outside, or strictly within, the region.

