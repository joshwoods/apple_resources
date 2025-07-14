

- Apple Search Ads
-  Search for Geolocations 

Web Service Endpoint

# Search for Geolocations

Fetches a list of geolocations for targeting.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/search/geo
```

## Query Parameters

`countrycode`

`string`

The country or region to serve ads in. Campaigns that serve multiple countries or regions can’t use geotargeting.

The query uses a `countrycode` value in an ISO alpha-2 country code format.

```
GET https://api.searchads.apple.com/api/v5/search/geo?countrycode=US
```

Default: `US`

`entity`

`string`

The `country`, `AdminArea`, or L`ocality` locations available for targeting.

An `AdminArea` is the state or the equivalent according to its associated country. A `Locality` is the city or the equivalent according to its associated `AdminArea`.

A `countrycode` is a mandatory parameter.

```
GET https://api.searchads.apple.com/api/v5/search/geo?entity=AdminArea&countrycode=US
```

```
GET https://api.searchads.apple.com/api/v5/search/geo?entity=Locality&countrycode=US
```

The `entity` query parameter searches the `displayNames` for `country`, `adminArea`, and `Locality` in all languages.

Search results in the response payload are in the preferred language according to your organization.

If you don’t input a query parameter, all applicable values return in the response payload as a default.

`limit`

`int32`

The limit on the number of geolocations in the response.

```
GET https://api.searchads.apple.com/api/v5/search/geo?limit=1000
```

Default: `20`

`offset`

`int32`

The offset pagination that limits the number of returned records. The start of each page is offset by the specified number. You can apply `offset` to most API calls, but not all GET endpoints support it.

Default: `0`

`query`

`string`

The `query` search pattern uses a prefix-matching algorithm. You can use spaces in search patterns. Prefixes require a minimum of three characters. If you’re sending a quoted search string, use HTML encoding.

```
GET https://api.searchads.apple.com/api/v5/search/geo?query=%22New%20H%22
```

Default: `*:*`

## Response Codes

` 200 ``OK`

SearchEntityListResponse

`OK`

If the call succeeds, the API returns the SearchEntity object in the response payload with an HTTP status code of `200` `(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to obtain App Store locations you can use to refine your target audience. Specify the criteria for a geolocation search using the geotargeting criteria CountryCriteria, AdminAreaCriteria, and LocalityCriteria, and then apply them to ad groups using Create an Ad Group and Update an Ad Group endpoints.

### Payload Example: Search for Geolocations

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/search/geo?entity=adminArea&countrycode=US
```

```
{
  "id": "US|CA",
  "entity": "AdminArea",
  "displayName": "California, United States",
  "countryOrRegion": "US",
  "adminArea": "CA",
  "locality": null
}

```

## See Also

### Search Geolocation Endpoints

Get a List of Geo Locations

Gets geolocation details using a geoidentifier.

