

- MapKit JS
- GeocoderResponse
-  results 

Instance Property

# results

An array of places that returns from a geocoder lookup or reverse lookup.

MapKit JS 5.0+

``` source
attribute Place[] results;
```

## Discussion

An object the system parses from the geocoder JSON response, which contains an array of places. Each Place has several properties.

If there’s no response, results is an empty array.

