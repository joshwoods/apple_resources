

- Apple Search Ads
-  Get Localized App Details 

Web Service Endpoint

# Get Localized App Details

Fetches the localized default product page for an app.

## URL

``` source
GET https://api.searchads.apple.com/api/v5/apps/{adamId}/locale-details
```

## Path Parameters

`adamId`

`int64`

 (Required) 

Your unique App Store app identifier.

## Response Codes

` 200 ``OK`

MediaLocaleDetailResponse

`OK`

If successful, the API returns a list of objects in the response payload with an HTTP status code of `200 (OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to return localized app details using your `adamId` in the resource path. Related objects: MediaLocaleDetail, MediaLocaleDetailResponse.

### Query Parameters

- expand: Detailed app asset details of a device. Use `true` for expanded values in the API response.

### Get localized app details example

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/apps/{adamId}/locale-details        
```

```
{
  "data": [
    {
      "language": "en-US",
      "appName": "Trip Trek",
      "shortDescription": "Trip Trek app.",
      "isPrimaryLocale": true,
      "subTitle": "Search for trips.",
      "appPreviewDeviceWithAssets": {
        "ipadPro": {
          "appPreviewDeviceFallBackDevices": null,
          "screenshots": [
            {
              "assetGenId": "…",
              "assetToken": "…",
              "assetUrl": "…",
              "appPreviewDevice": "…",
              "sortPosition": 1,
              "sourceHeight": 2732,
              "sourceWidth": 2048,
              "orientation": "PORTRAIT",
              "assetType": "SCREENSHOT",
              "checksum": "…",
              "pictureUrl": "…",
              "videoUrl": null,
              "assetDuplicationType": null
            }
          ],
          "appPreviews": null
        }
      }
    }
  ]
}
```

## See Also

### App Details

Get App Details

Fetches app metadata.

