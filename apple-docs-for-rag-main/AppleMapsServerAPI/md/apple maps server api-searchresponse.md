

- Apple Maps Server API
-  SearchResponse 

Object

# SearchResponse

An object that contains the search region and an array of place descriptions that a search returns.

Apple Maps Server API 1.2+

``` source
object SearchResponse
```

## Properties

`displayMapRegion`

SearchMapRegion

Represents a rectangular region on a map expressed as south-west and north-east points. More specifically south latitude, west longitude, north latitude and east longitude.

`paginationInfo`

SearchResponse.PaginationInfo

`results`

`[`SearchResponse.Place`]`

An array of SearchResponse.Place results.

## Topics

### Place information returned by a search

object SearchResponse.Place

A structure returned by a search that describes a place.

object SearchResponse.PaginationInfo

An object that returns a page of search responses.

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

object StructuredAddress

An object that describes the detailed address components of a place.

