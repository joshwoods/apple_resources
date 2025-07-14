

- MapKit JS
- mapkit.Geocoder
-  reverseLookup 

Instance Method

# reverseLookup

Converts a geographic coordinate to an address.

MapKit JS 5.0+

``` source
number reverseLookup(
 mapkit.Coordinate coordinate,
 function callback,
 optional GeocoderReverseLookupOptions options
);
```

## Parameters 

`coordinate`  

The coordinate to convert to a human-readable address. For example, `new` \`\`mapkit.Coordinate\`\`\`(37.37, -122.04)\`.

`callback`  

MapKit JS invokes this callback function with two arguments, `error` on failure and `data` on success. If you cancel the request before you receive a response, the framework doesn’t call this function.

- `error` (Error). Contains an error code and descriptive message.

- `data` (Object). An array of places named results, which is an object the system parses from a server-returned JSON response. Each place in results has a coordinate property and a formattedAddress property. results is an empty array if there isn’t a match.

`options`  

language is the only option that you can set for the reverse geocoder. For example, `{ language: 'fr-CA' }` tells the server to send results localized to Canadian French. If you set it, this option overrides the language you provide in the mapkit.Geocoder constructor.

## Return Value

A request ID that you can pass to cancel to stop a pending request.

## Discussion

Reverse geocoding converts geographic coordinates to the nearest human-readable address.

## See Also

### Getting geocoder results

lookup

Converts an address to geographic coordinates.

GeocoderLookupOptions

Options that constrain geocoder lookup results to a specific area or a specific language.

GeocoderReverseLookupOptions

An option that constrains reverse lookup results to a specific language.

GeocoderResponse

The response from a geocoder lookup or reverse lookup.

