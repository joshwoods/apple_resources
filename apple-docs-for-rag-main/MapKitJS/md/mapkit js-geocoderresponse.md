

- MapKit JS
-  GeocoderResponse 

Structure

# GeocoderResponse

The response from a geocoder lookup or reverse lookup.

MapKit JS 5.0+

``` source
dictionary GeocoderResponse {
 Place[] results;
};
```

## Mentioned in 

MapKit JS 5

## Overview

The `data` parameter of the lookup or reverseLookup callback function contains the geocoder response. MapKit JS parses the `data` object from the geocoder JSON response, which contains an array of Place objects.

If there’s no response, results is an empty array.

## Topics

### Response

results

An array of places that returns from a geocoder lookup or reverse lookup.

## See Also

### Getting geocoder results

lookup

Converts an address to geographic coordinates.

GeocoderLookupOptions

Options that constrain geocoder lookup results to a specific area or a specific language.

reverseLookup

Converts a geographic coordinate to an address.

GeocoderReverseLookupOptions

An option that constrains reverse lookup results to a specific language.

