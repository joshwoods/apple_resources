

- Apple Maps Server API
-  SearchResultType 

Type

# SearchResultType

An enumerated string that indicates the result type for the search autocomplete request.

Apple Maps Server API 1.2+

``` source
string SearchResultType
```

## Possible Values 

`poi`  

`address`  

`physicalFeature`  

`pointOfInterest`  

## Possible Values

poi  
A physical feature or a point of interest.

address  
An address such as a street address, suburb, city, state, or country.

physicalFeature  
A natural physical feature, such as a river, mountain, or delta.

pointOfInterest  
A point of interest such as a cafe or grocery store.

## See Also

### Searching

type AddressCategory

Search categories related to political geographical boundaries.

type SearchACResultType

An enumerated string that indicates the result type for the search request.

object AlternateIdsResponse

A list of alternate Place IDs and associated errors.

object AlternateIdsResponse.AlternateIds

Contains a list of alternate Place IDs for a given Place ID.

object PlacesResponse

A list of Place IDs and errors.

object PlacesResponse.PlaceLookupError

An error associated with a lookup call.

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

