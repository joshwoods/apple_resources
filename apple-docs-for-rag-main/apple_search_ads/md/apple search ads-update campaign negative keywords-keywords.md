

- Apple Search Ads
-  Update Campaign Negative Keywords 

Web Service Endpoint

# Update Campaign Negative Keywords

Updates negative keywords in a campaign.

Search Ads 5.0+

## URL

``` source
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/negativekeywords/bulk
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

To update campaign negative keywords, use the associated `campaignId` in the URI. The `id` in the payload must belong to a negative keyword that exists inside the campaign in the URI. Use `PAUSED` or `ACTIVE` values to update the `status` field. Use partial updates to edit a subset of object properties without having to include all object properties in the payload. For more information, see the Use Partial Updates section of Using Apple Search Ads API Functionality.

### Payload example: Update campaign negative keywords

- Request
- Response

```
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/negativekeywords/bulk

[
    {
        "id": 542370642,
        "adGroupId": 542317095,
        "text": "Update campaign negative keyword example 1",
        "status": "PAUSED",
        "matchType": "BROAD",
        "deleted": false
    },
    {
        "id": 542370643,
        "adGroupId": 542317095,
        "text": "Update campaign negative keyword example 2",
        "status": "PAUSED",
        "matchType": "EXACT",
        "deleted": false
    }
]
```

```
[
        {
            "id": 542370642,
            "campaignId": 542370539,
            "adGroupId": 542317095,
            "text": "Update campaign negative keyword example 1",
            "status": "PAUSED",
            "matchType": "BROAD",
            "modificationTime": "2024-04-08T21:15:57.643",
            "deleted": false
        },
        {
            "id": 542370643,
            "campaignId": 542370539,
            "adGroupId": 542317095,
            "text": "cUpdate campaign negative keyword example 2",
            "status": "PAUSED",
            "matchType": "EXACT",
            "modificationTime": "2024-04-08T21:13:57.874",
            "deleted": false
        }
    ]
```

## See Also

### Campaign Negative Keywords Endpoints

Create Campaign Negative Keywords

Creates negative keywords for a campaign.

Find Campaign Negative Keywords

Fetches negative keywords for campaigns.

Get a Campaign Negative Keyword

Fetches a specific negative keyword in a campaign.

Get All Campaign Negative Keywords

Fetches all negative keywords in a campaign.

Delete Campaign Negative Keywords

Deletes negative keywords from a campaign.

