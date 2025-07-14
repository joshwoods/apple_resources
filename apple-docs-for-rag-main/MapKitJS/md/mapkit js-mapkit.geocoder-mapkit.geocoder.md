

- MapKit JS
- mapkit.Geocoder
-  mapkit.Geocoder 

Initializer

# mapkit.Geocoder

Creates a geocoder object and sets optional language and user location properties.

MapKit JS 5.0+

``` source
new mapkit.Geocoder(
 optional GeocoderConstructorOptions options
);
```

## Mentioned in 

MapKit JS 5

## Discussion

To use geocoding, create an instance of mapkit.Geocoder. Optionally, you can set the language and getsUserLocation properties of a mapkit.Geocoder object on initialization, as the following examples shows:

```
var geocoder = new mapkit.Geocoder({
    language: "en-GB",
    getsUserLocation: true
});
```

## See Also

### Creating a geocoder object

GeocoderConstructorOptions

Initialization options for geocoder objects.

getsUserLocation

A Boolean value that indicates whether the geocoder returns results near the user’s location.

language

A language ID that determines the language to use for displaying addresses.

