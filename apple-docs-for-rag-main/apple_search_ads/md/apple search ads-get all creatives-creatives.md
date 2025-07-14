

- Apple Search Ads
-  Get All Creatives 

Web Service Endpoint

# Get All Creatives

Fetches all creatives within an organization.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/creatives
```

## Query Parameters

`limit`

`int32`

The number of items to return per request. The maximum is 1000 for most objects.

Default: `20`

`offset`

`int32`

The offset pagination that limits the number of returned records. The start of each page is offset by the specified number.

Default: `0`

## Response Codes

` 200 ``OK`

CreativeListResponse

`OK`

If the call succeeds, the API returns the CreativeListResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to fetch details of all assigned Creative objects for your organization.

### Payload example: Get all creatives

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/creatives
```

```
{
  "id": 94790778,
  "orgId": 42173330,
  "adamId": 918469737,
  "name": "Trip Trek CPP variation 1",
  "type": "CUSTOM_PRODUCT_PAGE",
  "state": "VALID",
  "stateReasons": [],
  "creationTime": "2024-11-08T21:53:35.036",
  "modificationTime": "2024-09-04T21:53:35.036",
  "productPageId": "00d99d1e-ee93-48fc-973e-7ffc0ddfced6"
}
```

## See Also

### Creative Endpoints

Create a Creative

Creates a creative object within an organization.

Find Creatives

Finds creatives within an organization.

Get a Creative

Fetches a creative by identifier.

