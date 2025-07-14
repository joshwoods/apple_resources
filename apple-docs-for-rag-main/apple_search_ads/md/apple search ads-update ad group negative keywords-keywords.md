

- Apple Search Ads
-  Update Ad Group Negative Keywords 

Web Service Endpoint

# Update Ad Group Negative Keywords

Updates negative keywords in an ad group.

Search Ads 5.0+

## URL

``` source
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/negativekeywords/bulk
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

`[`NegativeKeyword`]`

The request body that includes negative keyword details.

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

To update negative keywords, use the associated `campaignId` and `adgroupId` in the URI. The `id` in the payload must belong to a negative keyword that exists inside the ad group in the URI. Use `PAUSED` or `ACTIVE` values to update the `status` field. Use partial updates to edit a subset of object properties without having to include all object properties in the payload. For more information, see the Use Partial Updates section of Using Apple Search Ads API Functionality.

### Payload example: Update ad group negative keywords

- Request
- Response

```
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/negativekeywords/bulk

[
  {
    "id": "12345678",
    "status": "PAUSED"
  },
  {
    "id": "12345679",
    "status": "PAUSED"
  }
]

```

```
[
  {
    "id": 12345678,
    "campaignId": 542370539,
    "adGroupId": 427916203,
    "text": "Update ad group negative keyword example 1",
    "status": "PAUSED",
    "matchType": "BROAD",
    "modificationTime": "2024-04-08T22:08:42.618",
    "deleted": false
  },
  {
    "id": 12345679,
    "campaignId": 542370539,
    "adGroupId": 427916203,
    "text": "Update ad group negative keyword example 2",
    "status": "PAUSED",
    "matchType": "EXACT",
    "modificationTime": "2024-04-08T22:08:42.618",
    "deleted": false
  }
]
```

## See Also

### Ad Group Negative Keywords Endpoints

Create Ad Group Negative Keywords

Creates negative keywords in a specific ad group.

Find Ad Group Negative Keywords

Fetches negative keywords in a campaign’s ad groups.

Get an Ad Group Negative Keyword

Fetches a specific negative keyword in an ad group.

Get All Ad Group Negative Keywords

Fetches all negative keywords in ad groups.

Delete Ad Group Negative Keywords

Deletes negative keywords from an ad group.

