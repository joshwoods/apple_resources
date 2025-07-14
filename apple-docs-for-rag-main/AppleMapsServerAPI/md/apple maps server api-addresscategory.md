

- Apple Maps Server API
-  AddressCategory 

Type

# AddressCategory

Search categories related to political geographical boundaries.

Apple Maps Server API 1.2+

``` source
string AddressCategory
```

## Possible Values 

`Country`  

`AdministrativeArea`  

`SubAdministrativeArea`  

`Locality`  

`SubLocality`  

`PostalCode`  

## Possible Values

Country  
Countries and regions. AdministrativeArea The primary administrative divisions of countries or regions.

SubAdministrativeArea  
The secondary administrative divisions of countries or regions.

Locality  
Local administrative divisions, postal cities and populated places.

SubLocality  
Local administrative sub-divisions, postal city sub-districts, and neighborhoods.

PostalCode  
A code assigned to addresses for mail sorting and delivery.

## See Also

### Searching

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

