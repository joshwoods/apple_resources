

- MapKit JS
- mapkit.Geocoder
-  getsUserLocation 

Instance Property

# getsUserLocation

A Boolean value that indicates whether the geocoder returns results near the user’s location.

MapKit JS 5.0+

``` source
attribute boolean getsUserLocation;
```

## Discussion

When set to `true`, the geocoder returns results that are near the user’s current location. The default value is `false`.

## See Also

### Creating a geocoder object

mapkit.Geocoder

Creates a geocoder object and sets optional language and user location properties.

GeocoderConstructorOptions

Initialization options for geocoder objects.

language

A language ID that determines the language to use for displaying addresses.

