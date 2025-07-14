

- Apple Search Ads
-  Search for iOS apps 

Web Service Endpoint

# Search for iOS apps

Searches for iOS apps to promote in a campaign.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/search/apps
```

## Query Parameters

`limit`

`int32`

The number of items to return per request. The maximum is 1000.

```
GET https://api.searchads.apple.com/api/v5/search/apps?limit=100
```

Default: `20`

`offset`

`int32`

The offset pagination that limits the number of records returned. The start of each page is offset by the number specified. You can apply `offset` to most API calls, but not all GET endpoints support it.

```
GET https://api.searchads.apple.com/api/v5/search/apps?limit=&offset=
```

Default: `0`

`query`

`string`

 (Required) 

The query for a list of iOS apps using a matching prefix.

```
GET https://api.searchads.apple.com/api/v5/search/apps?query=Run%20Ke
```

The query search pattern uses a prefix-matching algorithm. You can use spaces in search patterns. Prefixes require a minimum of three characters. If you’re sending a quoted search string, use HTML encoding.

`returnOwnedApps`

`boolean`

The list of apps belonging to your organization.

```
GET https://api.searchads.apple.com/api/v5/search/apps?query=appexample&returnOwnedApps=true
```

Default: `false`

## Response Codes

` 200 ``OK`

AppInfoListResponse

`OK`

If the call succeeds, the API returns the AppInfo object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to search for iOS apps that you can promote in a campaign. You can use query parameters to fetch data. For more information, see the Use Query Parameters section of Using Apple Search Ads API Functionality.

An app search returns your `adamId`, which you can use in Create a Campaign in addition to the `AppDownloaderCriteria` in the TargetingDimensions payload. You can apply targeting dimensions to ad groups using Create an Ad Group or Update an Ad Group endpoints.

### Payload Example: Search for iOS apps

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/search/apps?query=apple&limit=1
```

```
[
  {
    "adamId": 427916203,
    "appName": "Trip Trek example app",
    "developerName": "example Apple developer",
    "countryOrRegionCodes": [
      "FR",
      "DE",
      "US",
      "NO",
      "MX",
      "GB",
      "CA",
      "SE",
      "AU"
    ]
  }
]
```

