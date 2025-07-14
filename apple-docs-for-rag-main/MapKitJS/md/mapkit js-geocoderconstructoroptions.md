

- MapKit JS
-  GeocoderConstructorOptions 

Structure

# GeocoderConstructorOptions

Initialization options for geocoder objects.

MapKit JS 5.0+

``` source
dictionary GeocoderConstructorOptions {
 string language;
 boolean getsUserLocation;
};
```

## Overview

You can optionally set the language and getsUserLocation properties of a mapkit.Geocoder object on initialization. Provide a dictionary of GeocoderConstructorOptions, as shown in the following code listing.

```
var geocoder = new mapkit.Geocoder({
    language: "en-GB",
    getsUserLocation: true
});
```

## Topics

### Initializing options

getsUserLocation

An initial Boolean value that indicates whether the geocoder returns results near the user’s location.

language

An initial value for the language ID, which determines the language to use for displaying addresses.

## See Also

### Creating a geocoder object

mapkit.Geocoder

Creates a geocoder object and sets optional language and user location properties.

getsUserLocation

A Boolean value that indicates whether the geocoder returns results near the user’s location.

language

A language ID that determines the language to use for displaying addresses.

