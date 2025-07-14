

- Apple Search Ads
-  Get All Targeting Keywords in an Ad Group 

Web Service Endpoint

# Get All Targeting Keywords in an Ad Group

Fetches all targeting keywords in ad groups.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/targetingkeywords
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

## Query Parameters

`limit`

`int32`

The number of items to return per request. The maximum is 1000 for most objects.

Default: `20`

`offset`

`int32`

The offset pagination that limits the number of returned records. The start of each page is offset by the specified number.

Default: `0`

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

To return all targeting keywords for a campaign, use the associated `campaignId` and `adgroupId` in the URI. You can also use a partial fetch. For more information, see the Use a Partial Fetch section of Using Apple Search Ads API Functionality.

### Payload example: Get all targeting keywords

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/targetingkeywords
```

```
[
        {
            "id": 542370642,
            "adGroupId": 542317095,
            "text": "targeting keyword example 1",
            "status": "ACTIVE",
            "matchType": "BROAD",
            "bidAmount": {
                "amount": "100",
                "currency": "USD"
            },
            "modificationTime": "2024-04-08T16:53:17.457",
            "deleted": false
        },
        {
            "id": 542370643,
            "adGroupId": 542317095,
            "text": "targeting keyword example 2",
            "status": "ACTIVE",
            "matchType": "BROAD",
            "bidAmount": {
                "amount": "100",
                "currency": "USD"
            },
            "modificationTime": "2024-04-08T20:48:28.206",
            "deleted": false
        },
        {
            "id": 542370644,
            "adGroupId": 542317095,
            "text": "targeting keyword example 3",
            "status": "PAUSED",
            "matchType": "BROAD",
            "bidAmount": {
                "amount": "2",
                "currency": "USD"
            },
            "modificationTime": "2023-04-08T21:02:24.257",
            "deleted": false
        },
        {
            "id": 542370645,
            "adGroupId": 542317095,
            "text": "targeting keyword example 4",
            "status": "ACTIVE",
            "matchType": "EXACT",
            "bidAmount": {
                "amount": "100",
                "currency": "USD"
            },
            "modificationTime": "2024-04-08T16:53:17.468",
            "deleted": false
        },
        {
            "id": 542370646,
            "adGroupId": 542317095,
            "text": "targeting keyword example 5",
            "status": "ACTIVE",
            "matchType": "EXACT",
            "bidAmount": {
                "amount": "100",
                "currency": "USD"
            },
            "modificationTime": "2023-04-08T17:53:10.899",
            "deleted": false
        },
        {
            "id": 542370647,
            "adGroupId": 542317095,
            "text": "targeting keyword example 6",
            "status": "PAUSED",
            "matchType": "EXACT",
            "bidAmount": {
                "amount": "100",
                "currency": "USD"
            },
            "modificationTime": "2024-04-08T21:02:24.267",
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

Update Targeting Keywords

Updates targeting keywords in ad groups.

Delete Targeting Keywords

Deletes targeting keywords from ad groups.

Delete a Targeting Keyword

Deletes a targeting keyword in an ad group.

