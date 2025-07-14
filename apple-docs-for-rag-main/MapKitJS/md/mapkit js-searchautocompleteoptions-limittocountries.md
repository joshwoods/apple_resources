

- MapKit JS
- SearchAutocompleteOptions
-  limitToCountries 

Instance Property

# limitToCountries

A string that constrains search results to within the provided countries.

MapKit JS 5.49+

``` source
attribute string limitToCountries;
```

## Discussion

The string is a comma-separated list of two-letter, ISO 3166-1 country and region codes. For example, to limit search results to Germany, Belgium, and France specify `de,be,fr`.

## See Also

### Autocomplete search filtering

includePhysicalFeatures

A Boolean value that indicates whether the autocomplete search results include physical features, such as mountain ranges, rivers, and ocean basins.

includePointsOfInterest

A Boolean value that indicates whether the search results include points of interest.

includeQueries

A Boolean value that indicates whether the search results include queries.

regionPriority

A filter that controls whether results occur outside, or strictly within, the region.

