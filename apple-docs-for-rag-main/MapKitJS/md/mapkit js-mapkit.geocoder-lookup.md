

- MapKit JS
- mapkit.Geocoder
-  lookup 

Instance Method

# lookup

Converts an address to geographic coordinates.

MapKit JS 5.0+

``` source
number lookup(
 string place,
 function callback,
 optional GeocoderLookupOptions options
);
```

## Parameters 

`place`  

A case-insensitive string MapKit JS converts to geographic coordinates, such as: “`450 Serra Mall`”, “`450 Serra Mall, Stanford`”, “`450 Serra Mall, Stanford, CA USA`”. Delimiter characters are optional.

`callback`  

MapKit JS returns geocoding results asynchronously through a callback function. MapKit JS invokes the callback function with two arguments, `error` on failure and `data` on success.

- `error` (Error). Contains an error code and descriptive message.

- `data` (Object). An array of places named results, which is an object the system parses from a server-returned JSON response. Each place in results has a coordinate property and a formattedAddress property. results is an empty array if there isn’t a match.

`options`  

The geocoder returns the most relevant results for a query. For example, a query for *Paris* returns results for Paris, France. Use GeocoderLookupOptions to constrain the search to specific countries, or to a desired area with a coordinate or region.

## Return Value

This method returns a request ID, which is an integer that you can pass to cancel to stop a pending request.

## Discussion

Geocoding converts a human-readable address to latitude and longitude coordinates. You can use mapkit.Geocoder to look up coordinates for a city, landmark, or address.

## See Also

### Getting geocoder results

GeocoderLookupOptions

Options that constrain geocoder lookup results to a specific area or a specific language.

reverseLookup

Converts a geographic coordinate to an address.

GeocoderReverseLookupOptions

An option that constrains reverse lookup results to a specific language.

GeocoderResponse

The response from a geocoder lookup or reverse lookup.

