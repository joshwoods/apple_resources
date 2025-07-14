

- MapKit JS
- GeocoderLookupOptions
-  limitToCountries 

Instance Property

# limitToCountries

A list of countries for constraining the lookup results.

MapKit JS 5.0+

``` source
attribute string limitToCountries;
```

## Discussion

This property tells the geocoder to return results within a list of countries. Specify countries in the list using two-letter ISO country codes. For example, constrain the geocoder to return results in Australia and New Zealand with `{ limitToCountries: "AU, NZ" }`.

## See Also

### Options

coordinate

Coordinates for constraining the lookup results.

language

The language to use when displaying the lookup results.

region

A region for constraining lookup results.

