

- Apple Search Ads
-  Find App Assets 

Web Service Endpoint

# Find App Assets

Fetches app asset metadata by adam ID.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/apps/{adamId}/assets/find
```

## Path Parameters

`adamId`

`int64`

 (Required) 

Your unique App Store app identifier.

Your `adamId` in the resource path needs to match the `adamId` in your campaign. Use Get a Campaign or Get all Campaigns to obtain your `adamId` and correlate it to the correct campaign.

## HTTP Body

Selector

The request body that includes the selector Condition. Selector objects define what data the API returns when fetching resources.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppAssetListResponse

`OK`

If the call succeeds, the API returns the AppAssetListResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Apple Search Ads Campaign Management API 4

## Discussion

Use this endpoint with Selector to find app asset metadata associated with an `adamId`. Use your `adamId` in the resource path. See the AppAsset object for parameter descriptions and selector condition operators.

This endpoint supports default and custom product page ads.

### Payload example: Find app assets

- Request
- Response

```
HTTP POST https://api.searchads.apple.com/api/v5/apps/{adamId}/assets/find

{
  “conditions”: [
    {
      “field”: “assetGenId”,
      “operator”: “equals”,
      “values”: [
        “368234568;en-US;9;0;4201c5a4bd4087cc82xdfetdc8141b94d0”
      ]
    }
  ]
}
```

```
{
  "data": [
    {
      "assetGenId": "368234568;en-US;9;0;4201c5a4bd4087cc82xdfetdc8141b94d0",
      "adamId": 835599320,
      "assetURL”: “https://is5-ssl.mzstatic.com/image/thumb/source113/v4/25/f5/70/25f57023-87bd-25f0-71dc-bf5f48525b4c/afcd3ec4-d7af-49c5-9d93-44084b0abea8_2208x1242iphone55_4.jpg/2208x1242.jpg",
      "assetVideoURL": null,
      "appPreviewDevice": “iphone_6_7”,
      "sourceHeight": 2208,
      "sourceWidth": 1242,
      "orientation": "PORTRAIT",
      "assetType": "SCREENSHOT"
    },
    {
      "assetGenId": "368234568;en-US;9;0;4201c5a4bd4087cc82xdfetdc8141b94d0",
      "adamId": 835599320,
      "assetURL”: “https://is5-ssl.mzstatic.com/image/thumb/PurpleSource122/v4/0b/d2/ea/0bd2ea96-744a-4341-2227-8aaa5c79ceef/84589e4f-d770-4444-9ade-e0806658f171_0.png/1290x2796.jpg",
      "assetVideoURL": null,
      "appPreviewDevice": "iphone_6_7",
      "sourceHeight": 1290,
      "sourceWidth": 2796,
      "orientation": “LANDSCAPE”,
      "assetType": “SCREENSHOT”
    }
 ],
  "pagination": {
    "totalResults": 2,
    "startIndex": 0,
    "itemsPerPage": 10
  }
}
```

## See Also

### Ad Rejections

Find Ad Creative Rejection Reasons

Fetches ad creative rejection reasons.

Get Ad Creative Rejection Reasons

Fetches ad creative rejection reasons by custom product page ID.

