

- Apple Maps Server API
-  AutocompleteResult 

Object

# AutocompleteResult

An object that contains information you can use to suggest addresses and further refine search results.

Apple Maps Server API 1.2+

``` source
object AutocompleteResult
```

## Properties

`completionUrl`

`string`

The relative URI to the `search` endpoint to use to fetch more details pertaining to the result. If available, the framework encodes opaque data about the autocomplete result in the completion URL’s `metadata` parameter.

If clients need to fetch the search result in a certain language, they’re responsible for specifying the `lang` parameter in the request.

`displayLines`

`[string]`

A JSON string array to use to create a long form of display text for the completion result.

`location`

Location

A Location object that specifies the location of the result in terms of its latitude and longitude.

`structuredAddress`

StructuredAddress

A StructuredAddress object that describes the detailed address components of a place.

## Discussion

If available, the service encodes opaque data about the autocomplete result in the completion URL’s `metadata` parameter. If you need to fetch the search result in a certain language, you need to specify it in the `lang` parameter in the request.

## See Also

### Getting common object information

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

object StructuredAddress

An object that describes the detailed address components of a place.

