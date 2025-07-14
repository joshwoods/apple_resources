

- MapKit JS
- SearchConstructorOptions
-  includeQueries 

Instance Property

# includeQueries

A Boolean value that indicates whether the search results include queries.

MapKit JS 5.32.2+

``` source
attribute boolean includeQueries;
```

## Discussion

This option only applies to search autocomplete. For example, if you send *cof* to autocomplete, the search returns only *coffee*. If you send *cof* to autocomplete while `includeQueries` is `false`, the search returns only addresses and points of interest (given that the setting for those options is `true`) related to *cof* and not necessarily related to *coffee*.

The default value is `true`.

## See Also

### Search filtering

includePhysicalFeatures

A Boolean value that indicates whether the search results include physical features, such as mountain ranges, rivers, and ocean basins.

limitToCountries

A string that constrains search results to within the provided countries.

regionPriority

A filter that controls whether results occur outside, or strictly within, the region.

