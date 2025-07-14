

- Apple Search Ads
-  Get App Preview Device Sizes 

Web Service Endpoint

# Get App Preview Device Sizes

Fetches supported app preview device-size mappings.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/creativeappmappings/devices
```

## Response Codes

` 200 ``OK`

AppPreviewDevicesMappingResponse

`OK`

If the call succeeds, the API returns the AppPreviewDevicesMappingResponse object in the response payload with an HTTP status code of `200(OK)`.

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

## Mentioned in 

Creative Sets

## Discussion

Use this endpoint to return a complete list of supported app preview device-size mappings.

### Payload example: Get app preview device sizes

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/creativeappmappings/devices
```

```
{
    "ipadPro": "iPad 12.9",
    "iphone6+": "iPhone 5.5",
    "iphone_5_8": "iPhone 5.8",
    "iphone5": "iPhone 4",
    "iphone6": "iPhone 4.7",
    "ipadPro_2018": "iPad 11",
    "ipad": "iPad 9.7",
    "iphone_6_5": "iPhone 6.5",
    "ipad_10_5": "iPad 10.5"
}
```

## See Also

### Product Page Endpoints

Get Product Pages

Fetches metadata of all your custom product pages.

Get Product Pages by Identifier

Fetches metadata for a specific product page.

Get Product Page Locales

Fetches product page locales by identifier.

Get Supported Countries or Regions

Fetches supported languages and language codes.

