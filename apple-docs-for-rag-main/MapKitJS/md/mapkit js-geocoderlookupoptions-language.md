

- MapKit JS
- GeocoderLookupOptions
-  language 

Instance Property

# language

The language to use when displaying the lookup results.

MapKit JS 5.0+

``` source
attribute string language;
```

## Discussion

Tell the geocoder to return results in this language. For example, setting the option `{ language: 'fr-CA' }` tells the server to send results localized to Canadian French. If you set it, this option overrides the language you provide in the mapkit.Geocoder constructor.

## See Also

### Options

coordinate

Coordinates for constraining the lookup results.

limitToCountries

A list of countries for constraining the lookup results.

region

A region for constraining lookup results.

