

- Apple Search Ads
-  Find Ad Creative Rejection Reasons 

Web Service Endpoint

# Find Ad Creative Rejection Reasons

Fetches ad creative rejection reasons.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/product-page-reasons/find
```

## HTTP Body

Selector

The request body that includes the selector Condition. Selector objects define what data the API returns when fetching resources.

Content-Type: application/json

## Response Codes

` 200 ``OK`

ProductPageReasonListResponse

`OK`

If the call succeeds, the API returns the ProductPageReasonListResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to find rejected approval reasons for ad creatives based on default or custom product page. See the ProductPageReason object for rejection reason code enumerations, parameter descriptions, and Selector condition operators.

### Payload example 1: Find ad creative rejection reasons

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/product-page-reasons/find

{
  "conditions": [
    {
      "field": "supplySources",
      "operator": "equals",
      "values": [
        "APPSTORE_TODAY_TAB"
      ]
    },
    {
      "field": "countriesOrRegions",
      "operator": "IN",
      "values": [
        "US"
      ]
    },
    {
      "field": "productPageId",
      "operator": "IN",
      "values": [
        "59f4948c-3726-4cfc-8915-6b09afb36d83",
        "0349277e-32f8-436b-980a-258c3aabf0ad"
      ]
    },
    {
      "orderBy": [
        {
          "field": "productPageId",
          "sortOrder": "ASCENDING"
        }
      ]
    }
  ]
}
```

```
{
  "data": [
    {
      "id": 4567890421,
      "adamId": 144714574,
      "productPageId": "59f4948c-3726-4cfc-8915-6b09afb36d83",
      "assetGenId": "368234568;en-US;9;0;4201c5a4bd4087cc82xdfetdc8141b94d0",
      "supplySource": "APPSTORE_TODAY_TAB",
      "countryOrRegion": "US",
      "languageCode": "en-US",
      "reasonType": "REJECTION_REASON",
      "reasonCode": "SUBTITLE_LANGUAGE_CONFLICT",
      "reasonLevel": "CUSTOM_PRODUCT_PAGE_LOCALE",
      "comment": "Custom comment for rejection."
    },
    {
      "id": 4837240452,
      "adamId": 144714574,
      "productPageId": "0349277e-32f8-436b-980a-258c3aabf0ad",
      "assetGenId": "835599320;en-AU;9;0;dbac55b222a61e1939f19f2640e48dfa",
      "supplySource": "APPSTORE_TODAY_TAB",
      "countryOrRegion": "US",
      "languageCode": "en-US",
      "reasonType": "APP_NAME_LANGUAGE_CONFLICT",
      "reasonCode": "CUSTOM_PRODUCT_PAGE_LOCALE",
      "comment": "Custom comment for rejection."
    }
  ],
  "pagination": {
    "totalResults": 2,
    "startIndex": 0,
    "itemsPerPage": 10
  }
}

```

### Payload example 2: Find ad creative rejection reasons

- Request
- Response

```
HTTP POST https://api.searchads.apple.com/api/v5/product-page-reasons/find

{
  "conditions": [
    {
      "field": "adamId",
      "operator": "equals",
      "values": [
        "735599345"
      ]
    },

      "orderBy": [
        {
          "field": "productPageId",
          "sortOrder": "ASCENDING"
        }
      ]
    }
  ]
}

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
    "languageCode": "en-US",
    "reasonType": "REJECTION_REASON",
    "reasonCode": "APP_NAME_LANGUAGE_CONFLICT",
    "reasonLevel": "CUSTOM_PRODUCT_PAGE_LOCALE",
    "comment”: "Custom comment for rejection."
  }
}
```

## See Also

### Ad Rejections

Get Ad Creative Rejection Reasons

Fetches ad creative rejection reasons by custom product page ID.

Find App Assets

Fetches app asset metadata by adam ID.

