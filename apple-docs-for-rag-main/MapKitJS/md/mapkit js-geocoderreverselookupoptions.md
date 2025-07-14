

- MapKit JS
-  GeocoderReverseLookupOptions 

Structure

# GeocoderReverseLookupOptions

An option that constrains reverse lookup results to a specific language.

MapKit JS 5.0+

``` source
dictionary GeocoderReverseLookupOptions {
 string language;
};
```

## Overview

Configure GeocoderReverseLookupOptions when performing a reverse lookup to constrain geocoder results to return results in a specific language.

## Topics

### Options

language

The language to use when displaying the reverse lookup results.

## See Also

### Getting geocoder results

lookup

Converts an address to geographic coordinates.

GeocoderLookupOptions

Options that constrain geocoder lookup results to a specific area or a specific language.

reverseLookup

Converts a geographic coordinate to an address.

GeocoderResponse

The response from a geocoder lookup or reverse lookup.

