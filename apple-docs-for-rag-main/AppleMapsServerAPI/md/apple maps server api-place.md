

- Apple Maps Server API
-  Place 

Object

# Place

An object that describes a place in terms of a variety of spatial, administrative, and qualitative properties.

Apple Maps Server API 1.2+

``` source
object Place
```

## Properties

`country`

`string`

The country or region of the place.

`countryCode`

`string`

The 2-letter country code of the place.

`displayMapRegion`

MapRegion

The geographic region associated with the place.

This is a rectangular region on a map expressed as south-west and north-east points. Specifically south latitude, west longitude, north latitude, and east longitude.

`formattedAddressLines`

`[string]`

The address of the place, formatted using its conventions of its country or region.

`name`

`string`

A place name that you can use for display purposes.

`coordinate`

Location

The latitude and longitude of this place.

`structuredAddress`

StructuredAddress

A StructuredAddress object that describes details of the place’s address.

`alternateIds`

`[string]`

A list of alternate Place IDs for the `id`.

`id`

`string`

An opaque string that identifies a place.

## Relationships

### Inherited By

- SearchResponse.Place

## See Also

### Getting common object information

object AutocompleteResult

An object that contains information you can use to suggest addresses and further refine search results.

object DirectionsResponse

An object that describes the directions from a starting location to a destination in terms routes, steps, and a series of waypoints.

object EtaResponse

An object that contains an array of one or more estimated times of arrival (ETAs).

object Location

An object that describes a location in terms of its longitude and latitude.

object MapRegion

An object that describes a map region in terms of its upper-right and lower-left corners as a pair of geographic points.

object PlaceResults

An object that contains an array of places.

object SearchAutocompleteResponse

An array of autocomplete results.

object SearchMapRegion

An object that describes an area to search in terms of its upper-right and lower-left corners as a pair of geographic points.

object SearchResponse

An object that contains the search region and an array of place descriptions that a search returns.

object StructuredAddress

An object that describes the detailed address components of a place.

