

- MapKit JS
-  mapkit.Search.RegionPriority 

Enumeration

# mapkit.Search.RegionPriority

A value that indicates the importance of the configured region.

MapKit JS 5.78.1+

``` source
interface mapkit.Search.RegionPriority {
 const string Default;
 const string Required;
};
```

## Topics

### Setting the region priority

Default

A value indicating that the results can originate from outside the specified region.

Required

A value indicating that no results can originate from outside the specified region.

## See Also

### Filtering a search

mapkit.AddressCategory

The categories of address components that users can search for with an address filter.

mapkit.AddressFilter

An object that filters which address options to include or exclude in search results.

