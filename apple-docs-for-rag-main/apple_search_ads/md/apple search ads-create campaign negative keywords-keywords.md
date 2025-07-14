

- Apple Search Ads
-  Create Campaign Negative Keywords 

Web Service Endpoint

# Create Campaign Negative Keywords

Creates negative keywords for a campaign.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/negativekeywords/bulk
```

## Path Parameters

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

## HTTP Body

`[`NegativeKeyword`]`

The request body that includes negative keyword details.

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

Negative keywords prevent your ad from showing up in App Store searches. Negative keywords can belong to a campaign or an ad group.

To create campaign negative keywords, use the associated `campaignId` in the URI.

### Payload example: Create campaign negative keywords

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/negativekeywords/bulk

[
    {
        "text": "create campaign negative keyword example 1",
        "matchType": "EXACT"
    },
    {
        "text": "create campaign negative keyword example 2",
        "matchType": "BROAD"
    }
]
```

```
[
  {
    "id": 542370642,
    "campaignId": 542370539,
    "adGroupId": 542317095,
    "text": "create campaign negative keyword example 1",
    "status": "ACTIVE",
    "matchType": "EXACT",
    "modificationTime": "2024-04-08T20:52:59.050",
    "deleted": false
  },
  {
    "id": 542370643,
    "campaignId": 542370539,
    "adGroupId": 542317095,
    "text": "create campaign negative keyword example 2",
    "status": "ACTIVE",
    "matchType": "BROAD",
    "modificationTime": "2024-04-08T20:52:59.054",
    "deleted": false
  }
]
```

## See Also

### Campaign Negative Keywords Endpoints

Find Campaign Negative Keywords

Fetches negative keywords for campaigns.

Get a Campaign Negative Keyword

Fetches a specific negative keyword in a campaign.

Get All Campaign Negative Keywords

Fetches all negative keywords in a campaign.

Update Campaign Negative Keywords

Updates negative keywords in a campaign.

Delete Campaign Negative Keywords

Deletes negative keywords from a campaign.

