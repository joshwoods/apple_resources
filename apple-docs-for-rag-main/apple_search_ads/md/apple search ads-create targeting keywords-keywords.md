

- Apple Search Ads
-  Create Targeting Keywords 

Web Service Endpoint

# Create Targeting Keywords

Creates targeting keywords in ad groups.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/targetingkeywords/bulk
```

## Path Parameters

`adgroupId`

`int64`

 (Required) 

The unique identifier for the ad group.

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

## HTTP Body

`[`Keyword`]`

The request body that includes keyword targeting details.

Content-Type: application/json

## Response Codes

` 200 ``OK`

KeywordListResponse

`OK`

If the call succeeds, the API returns a list of Keyword objects in the response payload with an HTTP status code of `200` `(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

Content-Type: application/json

` 400 ``Bad Request`

ApiErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ApiErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ApiErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ApiErrorResponse

`Not Found`

Content-Type: application/json

` 429 `

ApiErrorResponse

Content-Type: application/json

` 500 ``Internal Server Error`

ApiErrorResponse

`Internal Server Error`

Content-Type: application/json

## Overview

Note

If you create duplicate keywords, the payload response indicates an error, but the call returns with a 200 status code.

- 400: An invalid query or missing required parameters.

- 401: An unauthenticated call fails to get the requested response.

- 403: Insufficient rights to the resource.

- 404: The API can’t locate the resource.

- 429: The API calls exceed rate-limit thresholds. See the Rate Limits subsection of Calling the Apple Search Ads API.

- 500: The Apple Search Ads server is temporarily down or unreachable. The request may be valid, but you need to retry it later.

## Discussion

Keywords must belong to a specific ad group, unlike negative keywords, which can belong to a campaign or an ad group.

To create targeting keywords, use the associated `campaignId` and `adgroupId` in the URI.

Note

The limit is 5000 targeting keywords per campaign and per ad group.

### Payload example: Create ad group targeting keywords

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/targetingkeywords/bulk

[  
  {
    "text": "targeting keyword example 1",
    "matchType": "BROAD",
    "bidAmount": {
      "amount": "100",
      "currency": "USD"
    }
  },
  {
    "text": "targeting keyword example 2",
    "matchType": "EXACT",
    "bidAmount": {
      "amount": "100",
      "currency": "USD"
    }
  }
]

```

```
[
  {
    "id": 542370642,
    "adGroupId": 427916203,
    "text": “targeting keyword example 1””,
    "status": "ACTIVE",
    "matchType": "BROAD",
    "bidAmount": {
      "amount": "1.5",
      "currency": "USD"
    },
    "modificationTime": "2023-04-08T16:53:17.457",
    "deleted”: false
  },
  {
    "id": 542370642,
    "adGroupId": 427916203,
    "text": “targeting keyword example 2”,
    "status": “ACTIVE",
    "matchType": "EXACT",
    "bidAmount": {
      "amount": "2",
      "currency": "USD"
    },
    "modificationTime": "2024-04-08T16:53:17.468",
    "deleted": false
  }
]
```

## See Also

### Ad Group Targeting Keywords Endpoints

Find Targeting Keywords in a Campaign

Fetches targeting keywords in a campaign’s ad groups.

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

