

- Apple Maps Server API
-  DirectionsResponse 

Object

# DirectionsResponse

An object that describes the directions from a starting location to a destination in terms routes, steps, and a series of waypoints.

Apple Maps Server API 1.2+

``` source
object DirectionsResponse
```

## Properties

`destination`

Place

A Place object that describes the destination.

`origin`

Place

A Place result that describes the origin.

`routes`

`[`DirectionsResponse.Route`]`

An array of routes. Each route references steps based on indexes into the steps array.

`stepPaths`

`[`Location`]`

An array of step paths across all steps across all routes. Each step path is a single polyline represented as an array of points. You reference the step paths by index into the array.

`steps`

`[`DirectionsResponse.Step`]`

An array of all steps across all routes. You reference the route steps by index into this array. Each step in turn references its path based on indexes into the `stepPaths` array.

## Topics

### Steps and routes

object DirectionsResponse.Route

An object that represent the components of a single route.

object DirectionsResponse.Step

An object that represents a step along a route.

## See Also

### Getting common object information

object AutocompleteResult

An object that contains information you can use to suggest addresses and further refine search results.

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

object StructuredAddress

An object that describes the detailed address components of a place.

