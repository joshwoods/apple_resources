

- MapKit JS
- DirectionsResponse
-  origin 

Instance Property

# origin

An optional starting point for routing directions.

MapKit JS 5.55+

``` source
attribute mapkit.Coordinate?|Place? origin;
```

## Discussion

If you use mapkit.Coordinate to request directions with route, MapKit JS returns a `mapkit.Coordinate` in the direction’s response. If you use a string or a Place to request directions, the property may be `null` or a `Place` instance.

When MapKit JS returns a `Place` instance, it may contain additional details that weren’t included in the original item used to request directions.

## See Also

### Directions response

request

The request object associated with the direction’s response.

routes

An array of route objects.

destination

An optional end point for routing directions.

