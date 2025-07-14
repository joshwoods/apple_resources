

- Apple Maps Server API
-  Search for places that match specific criteria 

Web Service Endpoint

# Search for places that match specific criteria

Find places by name or by specific search criteria.

Apple Maps Server API 1.2+

## URL

``` source
GET https://maps-api.apple.com/v1/search
```

## Query Parameters

`q`

`string`

 (Required) 

The place to search for. For example, `q=eiffel tower`.

`excludePoiCategories`

`[`PoiCategory`]`

A comma-separated list of strings that describes the points of interest to exclude from the search results. For example, `excludePoiCategories=Restaurant,Cafe`.

See PoiCategory for a complete list of possible values.

`includePoiCategories`

`[`PoiCategory`]`

A comma-separated list of strings that describes the points of interest to include in the search results. For example, `includePoiCategories=Restaurant,Cafe`.

See PoiCategory for a complete list of possible values.

`limitToCountries`

`[string]`

A comma-separated list of two-letter ISO 3166-1 codes of the countries to limit the results to. For example, `limitToCountries=US,CA` limits the search to the United States and Canada.

If you specify two or more countries, the results reflect the best available results for some or all of the countries rather than everything related to the query for those countries.

`resultTypeFilter`

`[`SearchResultType`]`

A comma-separated list of strings that describes the kind of result types to include in the response. For example, `resultTypeFilter=Poi`.

`lang`

Lang

The language the server should use when returning the response, specified using a BCP 47 language code. For example, for English use `lang=en-US`. Defaults to `en-US`.

Default: `en-US`

`searchLocation`

SearchLocation

A location defined by the application as a hint. Specify the location as a comma-separated string containing the latitude and longitude. For example, `searchLocation=37.78,-122.42`.

`searchRegion`

SearchRegion

A region the app defines as a hint. Specify the region specified as a comma-separated string that describes the region in the form north-latitude,east-longitude,south-latitude,west-longitude. For example, `searchRegion=38,-122.1,37.5,-122.5`.

`userLocation`

UserLocation

The location of the user, specified as a comma-separated string that contains the latitude and longitude. For example, `userLocation=37.78,-122.42`.

Search may opt to use the `userLocation`, if specified, as a fallback for the `searchLocation`.

`searchRegionPriority`

`string`

A value that indicates the importance of the configured region.

Possible Values: `default, required`

`enablePagination`

`boolean`

A value that tells the server that we expect paginated results.

Default: `false`

`pageToken`

`string`

A value that indicates which page of results to return.

`includeAddressCategories`

`[`AddressCategory`]`

A comma-separated list of strings that describes the addresses to include in the search results. For example, `includeAddressCategories=SubLocality,PostalCode`. If you use this parameter, you must include `address` in `resultTypeFilter`. See AddressCategory for a complete list of possible values.

`excludeAddressCategories`

`[`AddressCategory`]`

A comma-separated list of strings that describes the addresses to exclude in the search results. For example, `excludeAddressCategories=Country,AdministrativeArea`. If you use this parameter, you must include `address` in `resultTypeFilter`. See AddressCategory for a complete list of possible values.

## Response Codes

` 200 ``OK`

SearchResponse

`OK`

Returns a SearchMapRegion that describes a region that encloses the results, and an array of SearchResponse objects that describes the results of the search.

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An ErrorResponse object that contains an error message and an array of strings that contain additional details about the error.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

An ErrorResponse object that contains an error message that indicates the Maps access token was missing or invalid, and an array of strings that contains additional details about the error.

Content-Type: application/json

` 429 `

ErrorResponse

An ErrorResponse object that indicates the call exceeds the daily service call quota for the authorization token presented. The app should try again later. If your app requires a larger daily quota, submit a quota increase request form.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorResponse

`Internal Server Error`

An ErrorResponse object that contains a server error message and an array of strings that describe additional details about the error.

Content-Type: application/json

## Discussion

### Example

- Request
- Response

```
curl -si -H "Authorization: Bearer " "https://maps-api.apple.com/v1/search?q=eiffel%20tower"
```

```
{
  "displayMapRegion": {
    "southLatitude": 48.856909736059606,
    "westLongitude": 2.2924737352877855,
    "northLatitude": 48.85963364504278,
    "eastLongitude": 2.2965897526592016
  },
  "results": [
    {
      "name": "Eiffel Tower",
      "formattedAddressLines": [
        "5 Avenue Anatole France",
        "75007 Paris",
        "France"
      ],
      "structuredAddress": {
        "administrativeArea": "Île-de-France",
        "locality": "Paris",
        "postCode": "75007",
        "subLocality": "Tour Eiffel-Champs de Mars",
        "thoroughfare": "Avenue Anatole France",
        "subThoroughfare": "5",
        "fullThoroughfare": "5 Avenue Anatole France",
        "areasOfInterest": [
          "Eiffel Tower",
          "Parc Du Champ De Mars"
        ],
        "dependentLocalities": [
          "7th arr.",
          "Tour Eiffel-Champs de Mars"
        ]
      },
      "country": "France",
      "countryCode": "FR",
      "coordinate": {
        "latitude": 48.85827172505176,
        "longitude": 2.294531782785587
      }
    }
  ]
}
```

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

object PlacesResponse.PlaceLookupError

An error associated with a lookup call.

Search for places that meet specific criteria to autocomplete a place search

Find results that you can use to autocomplete searches.

Search for a place using an identifier

Obtain a Place object for a given Place ID.

Search for places using mulitple identifiers

Obtain a set of Place objects for a given set of Place IDs.

Obtain a list of alternate place identifiers

Get a list of alternate Place IDs given one or more Place IDs.

