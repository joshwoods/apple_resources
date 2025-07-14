

- MapKit JS
- SearchConstructorOptions
-  region 

Instance Property

# region

A map region that provides a hint for the geographic area to search.

MapKit JS 5.0+

``` source
attribute mapkit.CoordinateRegion region;
```

## Discussion

This property specifies a region of a map in which to search. In a map application, this is typically the region displayed in the map.

```
{ region: map.region }
```

## See Also

### Search Initialization

coordinate

A map coordinate that provides a hint for the geographic area to search.

getsUserLocation

A Boolean value that indicates whether to limit the search results to the user’s location, according to the web browser.

language

A language ID that determines the language for the search results text.

