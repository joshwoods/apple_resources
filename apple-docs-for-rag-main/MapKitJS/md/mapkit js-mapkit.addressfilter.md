

- MapKit JS
-  mapkit.AddressFilter 

Class

# mapkit.AddressFilter

An object that filters which address options to include or exclude in search results.

MapKit JS 5.78.1+

``` source
interface mapkit.AddressFilter
```

## Overview

Use this object to filter search results by criteria, such as country, region, and municipality. See mapkit.AddressCategory for more information.

## Topics

### Configuring the filter

excluding

A list of categories to exclude from a search.

including

A list of categories to include in a search.

excludesCategory

A Boolean value that indicates whether to exclude a category from a search.

includesCategory

A Boolean value that indicates whether to include a category from a search.

excludingAllCategories

A value that excludes all address categories.

includingAllCategories

A value that includes all address categories.

## See Also

### Search

mapkit.AddressCategory

The categories of address components that users can search for with an address filter.

mapkit.Search

An object that retrieves map-based search results for a user-entered query.

