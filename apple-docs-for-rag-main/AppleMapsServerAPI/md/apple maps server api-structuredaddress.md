

- Apple Maps Server API
-  StructuredAddress 

Object

# StructuredAddress

An object that describes the detailed address components of a place.

Apple Maps Server API 1.2+

``` source
object StructuredAddress
```

## Properties

`administrativeArea`

`string`

The state or province of the place.

`administrativeAreaCode`

`string`

The short code for the state or area.

`areasOfInterest`

`[string]`

Common names of the area in which the place resides.

`dependentLocalities`

`[string]`

Common names for the local area or neighborhood of the place.

`fullThoroughfare`

`string`

A combination of thoroughfare and subthoroughfare.

`locality`

`string`

The city of the place.

`postCode`

`string`

The postal code of the place.

`subLocality`

`string`

The name of the area within the locality.

`subThoroughfare`

`string`

The number on the street at the place.

`thoroughfare`

`string`

The street name at the place.

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

object Place

An object that describes a place in terms of a variety of spatial, administrative, and qualitative properties.

object PlaceResults

An object that contains an array of places.

object SearchAutocompleteResponse

An array of autocomplete results.

object SearchMapRegion

An object that describes an area to search in terms of its upper-right and lower-left corners as a pair of geographic points.

object SearchResponse

An object that contains the search region and an array of place descriptions that a search returns.

