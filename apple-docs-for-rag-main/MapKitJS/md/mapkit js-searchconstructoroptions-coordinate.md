

- MapKit JS
- SearchConstructorOptions
-  coordinate 

Instance Property

# coordinate

A map coordinate that provides a hint for the geographic area to search.

MapKit JS 5.0+

``` source
attribute mapkit.Coordinate coordinate;
```

## Discussion

This property supplies coordinates as a reference for a search.

```
{ coordinate: new mapkit.Coordinate(37.37, -122.04) }
```

## See Also

### Search Initialization

getsUserLocation

A Boolean value that indicates whether to limit the search results to the user’s location, according to the web browser.

language

A language ID that determines the language for the search results text.

region

A map region that provides a hint for the geographic area to search.

