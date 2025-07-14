

- Apple Search Ads
-  Find Ad Group Negative Keywords 

Web Service Endpoint

# Find Ad Group Negative Keywords

Fetches negative keywords in a campaign’s ad groups.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/negativekeywords/find
```

## Path Parameters

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

## HTTP Body

Selector

Selector objects define what data the API returns when fetching resources.

Content-Type: application/json

## Response Codes

` 200 ``OK`

NegativeKeywordListResponse

`OK`

If the call succeeds, the API returns a list of NegativeKeyword objects in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to find negative keywords in different ad groups within the same campaign. Use the associated `campaignId` in the URI. Find calls use Selector Condition operators to narrow results. If you don’t specify any selector conditions, the API returns all negative keywords across all ad groups of the campaign. See the NegativeKeyword object for details about Selector `condition` operators per field.

### Payload example: Find ad group negative neywords

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/negativekeywords/find

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
      "adGroupId": 427916203,
      "text": "ad group negative keyword example 1",
      "status": "ACTIVE",
      "matchType": "BROAD",
      "modificationTime": "2024-04-08T17:49:30.393",
      "deleted": false
    },
    {
      "id": 542370643,
      "campaignId": 542370539,
      "adGroupId": 427916203,
      "text": "ad group negative keyword example 2",
      "status": "ACTIVE",
      "matchType": "EXACT",
      "modificationTime": "2024-04-08T17:49:30.399",
      "deleted": false
    },
    {
      "id": 542370644,
      "campaignId": 542370539,
      "adGroupId": 427916203,
      "text": "ad group negative keyword example 3",
      "status”: "ACTIVE",
      "matchType": "BROAD",
      "modificationTime": "2024-04-08T01:55:00.017",
      "deleted": false
    },
    {
      "id": 542370645,
      "campaignId": 542370539,
      "adGroupId": 427916203,
      "text": "ad group negative keyword example 4",
      "status": "ACTIVE",
      "matchType": "EXACT",
      "modificationTime": "2024-04-08T01:55:00.025",
      "deleted": false
    },
    {
      "id": 542370646,
      "campaignId": 542370539,
      "adGroupId": 427916203,
      "text": "ad group negative keyword example 5",
      "status": "ACTIVE",
      "matchType": "BROAD",
      "modificationTime": "2024-04-08T20:34:19.129",
      "deleted": false
    },
    {
      "id": 542370647,
      "campaignId": 542370539,
      "adGroupId": 427916203,
      "text": "ad group negative keyword example 6",
      "status": "ACTIVE",
      "matchType": "EXACT",
      "modificationTime": "2024-04-08T20:34:19.131",
      "deleted": false
    }
  ],
  "pagination": {
    "totalResults": 6,
    "startIndex": 1,
    "itemsPerPage": 10
  }
}
```

## See Also

### Ad Group Negative Keywords Endpoints

Create Ad Group Negative Keywords

Creates negative keywords in a specific ad group.

Get an Ad Group Negative Keyword

Fetches a specific negative keyword in an ad group.

Get All Ad Group Negative Keywords

Fetches all negative keywords in ad groups.

Update Ad Group Negative Keywords

Updates negative keywords in an ad group.

Delete Ad Group Negative Keywords

Deletes negative keywords from an ad group.

