

- Apple Search Ads
-  Find Creatives 

Web Service Endpoint

# Find Creatives

Finds creatives within an organization.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/creatives/find
```

## HTTP Body

Selector

The request body that includes the selector Condition. Selector objects define what data the API returns when fetching resources.

Content-Type: application/json

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

Use this endpoint to find creatives using a Selector Condition to filter results. If you don’t specify selector conditions, all creatives return in the response. See Creative for field descriptions and selector condition operators.

Values are case-sensitive strings. The `orderBy` selector supports the `Id` and `name` fields.

### Payload example: Find creatives

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/creatives/find

{
  "conditions": [
    {
      "field": "name",
      "operator": "CONTAINS",
      "values": [
        "Trip"
      ]
    }
  ]
}

```

```
{
  "data": [
    {
      "id": 573408745,
      "orgId": 39872140,
      "adamId": 899247664,
      "name": "Trip Trek custom product page variation 1",
      "type": "CUSTOM_PRODUCT_PAGE",
      "state": "VALID",
      "stateReasons": [],
      "creationTime": "2024-10-09T20:07:19.506Z",
      "modificationTime": "2024-10-18T20:07:19.506Z",
      "productPageId": "76659d7a-d146-43d3-b6b8-b7a12f74bf6b"
    },
    {
      "id": 75606108,
      "orgId": 39879640,
      "adamId": 1004806037,
      "name": "Trip Trek Creative Set variation 2",
      "type": "CREATIVE_SET",
      "state": "INVALID",
      "stateReasons": [],
      "creationTime": "2024-03-04T02:44:14.775",
      "modificationTime": "2024-08-17T01:16:37.827",
      "languageCode": "en_US"
    }
  ],
  “pagination”: {
    “totalResults”: 2,
    “startIndex”: 1,
    “itemsPerPage”: 10
  }
}
```

## See Also

### Creative Endpoints

Create a Creative

Creates a creative object within an organization.

Get a Creative

Fetches a creative by identifier.

Get All Creatives

Fetches all creatives within an organization.

