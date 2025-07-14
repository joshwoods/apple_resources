

- Apple Search Ads
-  Find Targeting Keywords in a Campaign 

Web Service Endpoint

# Find Targeting Keywords in a Campaign

Fetches targeting keywords in a campaign’s ad groups.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/targetingkeywords/find
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

KeywordListResponse

`OK`

If the call succeeds, the API returns a list of Keyword objects in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to find targeting keywords in different ad groups within the same campaign. Use the associated `campaignId` in the URI. Find calls use Selector Condition operators to narrow results. If you don’t specify any selector conditions in the payload, the API returns all keywords across all ad groups of the campaign. For more information about available selection condition operators to use, see the Keyword object.

### Payload example: Find targeting keywords in a campaign

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/targetingkeywords/find

{
  "pagination": {
    "offset": 0,
    "limit": 100
  },
  "orderBy": [
    {
      "field": "id",
      "sortOrder": "ASCENDING"
    }
  ],
  "conditions": [
    {
      "field": "deleted",
      "operator": "EQUALS",
      "values": [
        "false"
      ]
    }
  ]
}

```

```
{
  "data": [
    {
      "id": 542370642,
      "adGroupId": 427916203,
      "text": "targeting keyword example 1",
      "status": "PAUSED",
      "matchType": "BROAD",
      "bidAmount": {
        "amount": "100",
        "currency": "USD"
      },
      "modificationTime": "2024-04-08T21:03:02.216",
      "deleted": false
    },
    {
      "id": 542370642,
      "adGroupId": 427916203,
      "text": "targeting keyword example 2",
      "status": "ACTIVE",
      "matchType": "EXACT",
      "bidAmount": {
        "amount": "100",
        "currency": "USD"
      },
      "modificationTime": "2024-04-08T17:53:10.899",
      "deleted": false
    }
  ],
  "pagination": {
    "totalResults": 2,
    "startIndex": 1,
    "itemsPerPage": 10
  }
}
```

## See Also

### Ad Group Targeting Keywords Endpoints

Create Targeting Keywords

Creates targeting keywords in ad groups.

Get a Targeting Keyword in an Ad Group

Fetches a specific targeting keyword in an ad group.

Get All Targeting Keywords in an Ad Group

Fetches all targeting keywords in ad groups.

Update Targeting Keywords

Updates targeting keywords in ad groups.

Delete Targeting Keywords

Deletes targeting keywords from ad groups.

Delete a Targeting Keyword

Deletes a targeting keyword in an ad group.

