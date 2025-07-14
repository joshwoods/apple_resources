

- Apple Search Ads
-  Create a Creative 

Web Service Endpoint

# Create a Creative

Creates a creative object within an organization.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/creatives
```

## HTTP Body

`(`CustomProductPageCreative` | `DefaultProductPageCreative`)`

The request body that includes details of the Creative.

Content-Type: application/json

## Response Codes

` 200 ``OK`

CreativeResponse

`OK`

If the call succeeds, the API returns the `CreativeResponse` object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to create a Creative object within your organization using your `productPageId`.

### Payload example: Create a creative

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/creatives

{
  "adamId": 899247964,
  "name": "Trip Trek CPP variation",
  "type”: "CUSTOM_PRODUCT_PAGE",
  "productPageId": "45812c9b-c296-43d3-c6a0-c5a02f74bf6e"
}
```

```
{
    "id": 94895512,
    "orgId": 39872140,
    "adamId": 899247964,
    "name": "Trip Trek CPP variation",
    "type": "CUSTOM_PRODUCT_PAGE",
    "state": "VALID",
    "stateReasons": [],
    "creationTime": "2024-10-09T06:48:22.812Z",
    "modificationTime": "2024-107-09T06:48:22.812Z",
    "productPageId": "45812c9b-c296-43d3-c6a0-c5a02f74bf6e"
  }

```

## See Also

### Creative Endpoints

Find Creatives

Finds creatives within an organization.

Get a Creative

Fetches a creative by identifier.

Get All Creatives

Fetches all creatives within an organization.

