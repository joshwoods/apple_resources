

- Apple Search Ads
-  Get a List of Geo Locations 

Web Service Endpoint

# Get a List of Geo Locations

Gets geolocation details using a geoidentifier.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/search/geo
```

## Query Parameters

`limit`

`int32`

The limit on the number of geolocations in the response.

```
POST https://api.searchads.apple.com/api/v5/search/geo?limit=100
```

Default: `20`

`offset`

`int32`

The offset pagination that limits the number of returned records. The start of each page is offset by the specified number. You can apply `offset` to most API calls, but not all GET endpoints support it.

```
POST https://api.searchads.apple.com/api/v5/search/geo?offset=
```

Default: `0`

## HTTP Body

`[`GeoRequest`]`

The georequest body.

Content-Type: application/json

## Response Codes

` 200 ``OK`

SearchEntityListResponse

`OK`

If the call succeeds, the API returns a list of SearchEntity objects in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

Content-Type: application/json

` 400 ``Bad Request`

ApiErrorResponse

`Bad Request`

An invalid query or missing required parameters.

Content-Type: application/json

` 401 ``Unauthorized`

ApiErrorResponse

`Unauthorized`

An unauthenticated call fails to get the requested response.

Content-Type: application/json

` 403 ``Forbidden`

ApiErrorResponse

`Forbidden`

Insufficient rights to the resource.

Content-Type: application/json

` 404 ``Not Found`

ApiErrorResponse

`Not Found`

The API can’t locate the resource.

Content-Type: application/json

` 429 `

ApiErrorResponse

The API calls exceed rate-limit thresholds. See the Rate Limits subsection of Calling the Apple Search Ads API.

Content-Type: application/json

` 500 ``Internal Server Error`

ApiErrorResponse

`Internal Server Error`

The Apple Search Ads server is temporarily down or unreachable. The request may be valid, but you need to retry it later.

Content-Type: application/json

## Discussion

Use a geo `id` in the request payload to return a corresponding `displayName` and geolocation.

### Payload Example: Get a list of geolocations

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/search/geo

[
  {
    "id": "US|CA|Cupertino",
    "entity": "locality"
  }
]
```

```
{
  "id": "US||CA|Cupertino",
  "entity": "locality",
  "displayName": "Cupertino, California, United States",
  "countryOrRegion”: "US",
  "adminArea”: "CA",
  "locality": "Cupertino"
}
```

## See Also

### Search Geolocation Endpoints

Search for Geolocations

Fetches a list of geolocations for targeting.

