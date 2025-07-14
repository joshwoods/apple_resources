

- Apple Maps Server API
- PlacesResponse
-  PlacesResponse.PlaceLookupError 

Object

# PlacesResponse.PlaceLookupError

An error associated with a lookup call.

Apple Maps Server API 1.2+

``` source
object PlacesResponse.PlaceLookupError
```

## Properties

`errorCode`

`string`

An error code that indicates whether an Place ID is invalid because it’s malformed, not found, or resulted in any other error.

Possible Values: `FAILED_INVALID_ID, FAILED_NOT_FOUND, FAILED_INTERNAL_ERROR`

`id`

`string`

The Place ID.

## See Also

### Searching

type AddressCategory

Search categories related to political geographical boundaries.

type SearchACResultType

An enumerated string that indicates the result type for the search request.

type SearchResultType

An enumerated string that indicates the result type for the search autocomplete request.

object AlternateIdsResponse

A list of alternate Place IDs and associated errors.

object AlternateIdsResponse.AlternateIds

Contains a list of alternate Place IDs for a given Place ID.

object PlacesResponse

A list of Place IDs and errors.

Search for places that match specific criteria

Find places by name or by specific search criteria.

Search for places that meet specific criteria to autocomplete a place search

Find results that you can use to autocomplete searches.

Search for a place using an identifier

Obtain a Place object for a given Place ID.

Search for places using mulitple identifiers

Obtain a set of Place objects for a given set of Place IDs.

Obtain a list of alternate place identifiers

Get a list of alternate Place IDs given one or more Place IDs.

