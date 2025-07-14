

- Apple Search Ads
-  Find Ads 

Web Service Endpoint

# Find Ads

Finds ads within a campaign by selector criteria.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/ads/find
```

## Path Parameters

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

## HTTP Body

Selector

The request body that includes the selector Condition. Selector objects define what data the API returns when fetching resources.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AdListResponse

`OK`

If the call succeeds, the API returns the AdListResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to find `ads` within campaigns using a Selector Condition to filter results. If you don’t specify selector conditions, all Ad objects return in the response. See the Ad object for parameter descriptions and selector condition operators.

### Payload example: Find ads

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/ads/find

{
  "conditions": [
    {
      "field": "creativeType",
      "operator": "EQUALS",
      "values": [
        "CUSTOM_PRODUCT_PAGE"
      ]
    },
    {
      "field": "status",
      "operator": "EQUALS",
      "values": [
        "PAUSED"
      ]
    }
  ],
  "fields": null,
  "orderBy": [
    {
      "field": "creativeType",
      "sortOrder": "ASCENDING"
    }
  ],
  "pagination": {
    "limit": 20,
    "offset": 0
  }
}
```

```
{
  "data": [
    {
      "id": 573408745,
      "orgId": 39872140,
      "campaignId": 570798765,
      "adGroupId": 440797654,
      "creativeId": 94895512,
      "name": "Trip Trek custom product page variation",
      "creativeType": "CUSTOM_PRODUCT_PAGE",
      "status": "PAUSED",
      "servingStatus": "NOT_RUNNING",
      "servingStateReasons": [
        "PAUSED_BY_USER"
      ],
      "deleted": false,
      "creationTime": "2024-10-08T00:03:47.889Z",
      "modificationTime": "2024-10-09T00:03:47.889Z"
    }
  ],
  "pagination": {
    "totalResults": 1,
    "startIndex": 1,
    "itemsPerPage": 10
  }
}
```

## See Also

### Ad Endpoints

Create an Ad

Creates an ad in an ad group with a creative.

Find Ads (org-level)

Fetches ads within an organization by selector criteria.

Get an Ad

Fetches an ad assigned to an ad group by identifier.

Get All Ads

Fetches all ads assigned to an ad group.

Update an Ad

Updates an ad in an ad group.

Delete an Ad

Deletes an ad from an ad group.

