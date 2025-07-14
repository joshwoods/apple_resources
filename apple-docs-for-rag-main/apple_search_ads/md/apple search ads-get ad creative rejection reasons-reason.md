

- Apple Search Ads
-  Get Ad Creative Rejection Reasons 

Web Service Endpoint

# Get Ad Creative Rejection Reasons

Fetches ad creative rejection reasons by custom product page ID.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/product-page-reasons/{productPageReasonId}
```

## Path Parameters

`productPageReasonId`

`int64`

 (Required) 

A unique identifier for a custom product page with an associated ad creative rejection reason.

## Response Codes

` 200 ``OK`

ProductPageReasonResponse

`OK`

If the call succeeds, the API returns the ProductPageReasonResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

Use this endpoint to fetch rejected ad creative approval reason details. Use the `id` that returns in `ProductPageReason` in the resource path as your `productPageReasonId`. See the ProductPageReason object for rejection reason code enumerations, parameter descriptions, and selector condition operators.

### Payload example: Get rejection reasons

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/product-page-reasons/{productPageReasonId}
```

```
{
  "data": {
    "id": "135366",
    "adamId": 735599345,
    "productPageId": "68e5948c-3726-4cfc-8915-6b09afb36d83",
    "assetGenId": "735599345;en-US;9;0;4201c5a4bd4087cc82xdfetdc8141b94d0",
    "supplySource": "APPSTORE_TODAY_TAB",
    "countryOrRegion": "US",
    "languageCode": “en-US”,
    "reasonType": "APP_NAME_LANGUAGE_CONFLICT",
    "reasonCode": "SUBTITLE_LANGUAGE_CONFLICT",
    "comment": null
  }
}
```

## See Also

### Ad Rejections

Find Ad Creative Rejection Reasons

Fetches ad creative rejection reasons.

Find App Assets

Fetches app asset metadata by adam ID.

