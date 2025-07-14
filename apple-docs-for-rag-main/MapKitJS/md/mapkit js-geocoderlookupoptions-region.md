

- MapKit JS
- GeocoderLookupOptions
-  region 

Instance Property

# region

A region for constraining lookup results.

MapKit JS 5.0+

``` source
attribute mapkit.CoordinateRegion region;
```

## Discussion

Tell the geocoder to return results in this region. For example, constrain the geocoder to return results in the region currently displayed by the map with `{ region: map.region }`.

## See Also

### Options

coordinate

Coordinates for constraining the lookup results.

language

The language to use when displaying the lookup results.

limitToCountries

A list of countries for constraining the lookup results.

