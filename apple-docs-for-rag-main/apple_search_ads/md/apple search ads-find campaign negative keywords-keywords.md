

- Apple Search Ads
-  Find Campaign Negative Keywords 

Web Service Endpoint

# Find Campaign Negative Keywords

Fetches negative keywords for campaigns.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/negativekeywords/find
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

NegativeKeywordListResponse

`OK`

If the call succeeds, the API returns a list of NegativeKeyword objects in the response payload with an HTTP status code of `200` `(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to find campaign negative keywords. Use the associated `campaignId` in the URI. Find calls use Selector Condition operators to narrow results. If you don’t specify any selector conditions, all negative keywords in the campaign return in the response. See the NegativeKeyword object for details about selector Condition operators per field.

### Payload example: Find campaign negative keywords

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/negativekeywords/find

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
      "campaignId": 542370539,
      "adGroupId": 542317095,
      "text": "Find campaign negative keywords example 1",
      "status": "ACTIVE",
      "matchType": "BROAD",
      "modificationTime": "2023-04-08T17:48:31.979",
      "deleted": false
    },
    {
      "id": 542370643,
      "campaignId": 542370539,
      "adGroupId": 542317095,
      "text": "Find campaign negative keywords example 2",
      "status": "ACTIVE",
      "matchType": "EXACT",
      "modificationTime": "2023-04-08T17:48:31.984",
      "deleted": false
    },
    {
      "id": 542370644,
      "campaignId": 542370539,
      "adGroupId": 542317095,
      "text": "Find campaign negative keywords example 3",
      "status": "ACTIVE",
      "matchType": "EXACT",
      "modificationTime": "2023-04-08T20:52:59.050",
      "deleted": false
    },
    {
      "id": 542370645,
      "campaignId": 542370539,
      "adGroupId": 542317095,
      "text": "Find campaign negative keywords example 4",
      "status": "ACTIVE",
      "matchType": "BROAD",
      "modificationTime": "2023-04-08T20:52:59.054",
      "deleted": false
    }
  ],
  "pagination": {
    "totalResults": 4,
    "startIndex": 1,
    "itemsPerPage": 10
  }
}
```

## See Also

### Campaign Negative Keywords Endpoints

Create Campaign Negative Keywords

Creates negative keywords for a campaign.

Get a Campaign Negative Keyword

Fetches a specific negative keyword in a campaign.

Get All Campaign Negative Keywords

Fetches all negative keywords in a campaign.

Update Campaign Negative Keywords

Updates negative keywords in a campaign.

Delete Campaign Negative Keywords

Deletes negative keywords from a campaign.

