

- MapKit JS
- GeocoderReverseLookupOptions
-  language 

Instance Property

# language

The language to use when displaying the reverse lookup results.

MapKit JS 5.0+

``` source
attribute string language;
```

## Discussion

language is the only option that you can set for the reverse geocoder. For example, `{ language: 'fr-CA' }` tells the server to send results localized to Canadian French. If you set it, this option overrides the language you provide in the Geocoder constructor.

