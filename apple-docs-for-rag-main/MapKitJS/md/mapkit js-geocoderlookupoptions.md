

- MapKit JS
-  GeocoderLookupOptions 

Structure

# GeocoderLookupOptions

Options that constrain geocoder lookup results to a specific area or a specific language.

MapKit JS 5.0+

``` source
dictionary GeocoderLookupOptions {
 string language;
 mapkit.Coordinate coordinate;
 mapkit.CoordinateRegion region;
 string limitToCountries;
};
```

## Overview

Configure GeocoderLookupOptions when performing a lookup to constrain geocoder results to a specific area or return results in a specific language.

## Topics

### Options

coordinate

Coordinates for constraining the lookup results.

language

The language to use when displaying the lookup results.

limitToCountries

A list of countries for constraining the lookup results.

region

A region for constraining lookup results.

## See Also

### Getting geocoder results

lookup

Converts an address to geographic coordinates.

reverseLookup

Converts a geographic coordinate to an address.

GeocoderReverseLookupOptions

An option that constrains reverse lookup results to a specific language.

GeocoderResponse

The response from a geocoder lookup or reverse lookup.

