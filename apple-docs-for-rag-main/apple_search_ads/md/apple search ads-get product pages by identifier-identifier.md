

- Apple Search Ads
-  Get Product Pages by Identifier 

Web Service Endpoint

# Get Product Pages by Identifier

Fetches metadata for a specific product page.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/apps/{adamId}/product-pages/{productPageId}
```

## Path Parameters

`adamId`

`int64`

 (Required) 

Your unique App Store app identifier.

Your `adamId` in the resource path must match the `adamId` in your campaign. Use Get a Campaign or Get all Campaigns to obtain your `adamId` and correlate it to the correct campaign.

`productPageId`

`string`

 (Required) 

A unique string to identify a product page on App Store Connect. For example, `45812c9b-c296-43d3-c6a0-c5a02f74bf6e`.

## Response Codes

` 200 ``OK`

ProductPageDetailResponse

`OK`

If the call succeeds, the API returns the ProductPageDetailResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to fetch metadata assigned to a specific product page using your `adamId` and `productPageId` in the resource path. Your `productPageId` is an identifier appended to your app product page. For example, `https://apps.apple.com/us/app/trip-trek/id12345678?45812c9b-c296-43d3-c6a0-c5a02f74bf6e`.

Use your `productPageId` to create a Creative and obtain a `creativeId`. See Create a Creative.

### Payload example: Get product pages by identifier

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/apps/{adamId}/product-pages/{productPageId}
```

```
    {
      "id”: "45812c9b-c296-43d3-c6a0-c5a02f74bf6e0",
      "name”: "Trip Trek CPP variation",
      "state": "VISIBLE",
      "adamId": 8992479644,
      "creationTime": "2024-10-25T23:59:59.000",
      "modificationTime": "2024-10-25T23:59:59.000"
    }
```

## See Also

### Product Page Endpoints

Get Product Pages

Fetches metadata of all your custom product pages.

Get Product Page Locales

Fetches product page locales by identifier.

Get Supported Countries or Regions

Fetches supported languages and language codes.

Get App Preview Device Sizes

Fetches supported app preview device-size mappings.

