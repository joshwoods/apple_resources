

- MapKit JS
- mapkit.Geocoder
-  language 

Instance Property

# language

A language ID that determines the language to use for displaying addresses.

MapKit JS 5.0+

``` source
attribute string language;
```

## Discussion

When you set the language attribute to a language ID (such as `fr-CA` or `en-GB`), the geocoder returns addresses in this language, if available. If language isn’t set when initializing a mapkit.Geocoder object, then the geocoder uses the language provided when you initialized mapkit.

The default value is `null`. The language can be unset by setting language to `null` or `undefined`.

## See Also

### Creating a geocoder object

mapkit.Geocoder

Creates a geocoder object and sets optional language and user location properties.

GeocoderConstructorOptions

Initialization options for geocoder objects.

getsUserLocation

A Boolean value that indicates whether the geocoder returns results near the user’s location.

