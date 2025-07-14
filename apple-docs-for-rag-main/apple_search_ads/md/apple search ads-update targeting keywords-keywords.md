

- Apple Search Ads
-  Update Targeting Keywords 

Web Service Endpoint

# Update Targeting Keywords

Updates targeting keywords in ad groups.

Search Ads 5.0+

## URL

``` source
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/targetingkeywords/bulk
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

`[`KeywordUpdateRequest`]`

The request body that includes keyword targeting details.

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

## Discussion

To update targeting keywords, use the associated `campaignId` and `adgroupId` in the URI. The `id` in the payload must belong to a keyword that exists inside the ad group in the URI. The `status` and `bidAmount` fields are modifiable in the payload. Use partial updates to edit a subset of object properties without having to include all object properties in the payload. For more information, see the Use Partial Updates section of Using Apple Search Ads API Functionality.

### Payload example: Update ad group targeting keywords

- Request
- Response

```
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/targetingkeywords/bulk

[  
  {
    "id": "542370642",
    "status": "PAUSED",
    "bidAmount": {
      "amount”: "100",
      "currency": "USD"
    }
  },
  {
    "id": "542370643",
    "status": "PAUSED",
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
    "text": "targeting keyword example 1",
    "status": "PAUSED",
    "matchType": "BROAD",
    "bidAmount": {
      "amount": "100",
      "currency": "USD"
    },
    "modificationTime": "2023-04-08T21:02:24.257",
    "deleted": false
  },
  {
    "id": 542370643,
    "adGroupId": 427916203,
    "text": "targeting keyword example 2",
    "status": "PAUSED",
    "matchType": "EXACT",
    "bidAmount": {
      "amount": "100",
      "currency": "USD"
    },
    "modificationTime": "2023-04-08T21:02:24.267",
    "deleted": false
  }
]
```

## See Also

### Ad Group Targeting Keywords Endpoints

Create Targeting Keywords

Creates targeting keywords in ad groups.

Find Targeting Keywords in a Campaign

Fetches targeting keywords in a campaign’s ad groups.

Get a Targeting Keyword in an Ad Group

Fetches a specific targeting keyword in an ad group.

Get All Targeting Keywords in an Ad Group

Fetches all targeting keywords in ad groups.

Delete Targeting Keywords

Deletes targeting keywords from ad groups.

Delete a Targeting Keyword

Deletes a targeting keyword in an ad group.

