

- MapKit JS
- GeocoderLookupOptions
-  coordinate 

Instance Property

# coordinate

Coordinates for constraining the lookup results.

MapKit JS 5.0+

``` source
attribute mapkit.Coordinate coordinate;
```

## Discussion

Tell the geocoder to return results around this coordinate. For example, constrain the geocoder to return results around the coordinate 37.37, -122.04 with `{ coordinate: new mapkit.Coordinate(37.37, -122.04) }`.

## See Also

### Options

language

The language to use when displaying the lookup results.

limitToCountries

A list of countries for constraining the lookup results.

region

A region for constraining lookup results.

