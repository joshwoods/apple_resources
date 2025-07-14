

- Apple Search Ads
-  Get Product Pages 

Web Service Endpoint

# Get Product Pages

Fetches metadata of all your custom product pages.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/apps/{adamId}/product-pages
```

## Path Parameters

`adamId`

`int64`

 (Required) 

The unique identifier for the ad group.

## Query Parameters

`name`

`string`

Filters by `name` field. For example, the name of your custom product page on App Store Connect.

`states`

`string`

Filters by `states`, which indicates whether the product page is visible or not.

Possible Values: `HIDDEN, VISIBLE`

## Response Codes

` 200 ``OK`

ProductPageDetailListResponse

`OK`

If the call succeeds, the API returns the ProductPageDetailListResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Apple Search Ads Campaign Management API 5

## Discussion

Use this endpoint to fetch your product page metadata using your `adamId` in the resource path. Use your `productPageId` to Create a Creative obtain a `creativeId`.

### Payload example: Get product pages

The `id` in the response is your `productPageId`, an identifier for your app product page. For example, `45812c9b-c296-43d3-c6a0-c5a02f74bf6e`.

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/apps/{adamId}/product-pages
```

```

    {
      "id": "45812c9b-c296-43d3-c6a0-c5a02f74bf6e",
      "name": "Trip Trek CPP variation 1",
      "state": "VISIBLE",
      "adamId": 899247964,
      "creationTime": "2024-10-25T23:59:59.000",
      "modificationTime": "2024-10-08T17:44:49.718Z"
   }
```

## See Also

### Product Page Endpoints

Get Product Pages by Identifier

Fetches metadata for a specific product page.

Get Product Page Locales

Fetches product page locales by identifier.

Get Supported Countries or Regions

Fetches supported languages and language codes.

Get App Preview Device Sizes

Fetches supported app preview device-size mappings.

