

- MapKit JS
- GeocoderConstructorOptions
-  language 

Instance Property

# language

An initial value for the language ID, which determines the language to use for displaying addresses.

MapKit JS 5.0+

``` source
attribute string language;
```

## Discussion

If you don’t set language during initialization, the geocoder uses the value you provide during MapKit initialization (language).

Use standard two-letter ISO language IDs and two-letter region designators.

## See Also

### Initializing options

getsUserLocation

An initial Boolean value that indicates whether the geocoder returns results near the user’s location.

