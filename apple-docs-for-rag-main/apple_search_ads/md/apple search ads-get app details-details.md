

- Apple Search Ads
-  Get App Details 

Web Service Endpoint

# Get App Details

Fetches app metadata.

## URL

``` source
GET https://api.searchads.apple.com/api/v5/apps/{adamId}
```

## Path Parameters

`adamId`

`int64`

 (Required) 

Your unique App Store app identifier.

## Response Codes

` 200 ``OK`

MediaDetailResponse

`OK`

If the call succeeds, the API returns a response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

Content-Type: application/json

` 400 ``Bad Request`

ApiErrorResponse

`Bad Request`

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

Apple Search Ads Campaign Management API 5

## Discussion

Use this endpoint to return app details using your adamId in the resource path. Related objects: MediaDetail, MediaDetailResponse.

### Get app details example

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/apps/{adamId}
```

```
{
  "data": {
    "id": 284815942,
    "adamId": 284815942,
    "appName": "Trip Trek",
    "artistName": "Trip Trek",
    "primaryLanguage": "en-US",
    "primaryGenre": ">Mobile Software Applications>Utilities",
    "secondaryGenre": ">Mobile Software Applications>Reference",
    "deviceClasses": [
      "IPHONE",
      "IPAD"
    ],
    "iconPictureUrl": "...",
    "isPreOrder": "false",
    "availableStorefronts": [
      "US"
    ]
  }
}
```

## See Also

### App Details

Get Localized App Details

Fetches the localized default product page for an app.

