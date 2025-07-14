

- Apple Search Ads
-  Get All Campaign Negative Keywords 

Web Service Endpoint

# Get All Campaign Negative Keywords

Fetches all negative keywords in a campaign.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/negativekeywords
```

## Path Parameters

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

NegativeKeywordListResponse

`OK`

If the call succeeds, the API returns a list of NegativeKeyword objects in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

To return all campaign negative keywords, use the associated `campaignId` in the URI. You can also use a partial fetch. For more information, see the Use a Partial Fetch section of Using Apple Search Ads API Functionality.

### Payload example: Get all campaign negative keywords

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/negativekeywords
```

```
[
        {
            "id": 542370642,
            "campaignId": 542370539,
            "adGroupId": 427916203,
            "text": "Get campaign negative keyword example 1",
            "status": "ACTIVE",
            "matchType": "BROAD",
            "modificationTime": "2024-04-08T17:48:31.979",
            "deleted": false
        },
        {
            "id": 542370643,
            "campaignId": 542370539,
            "adGroupId": 427916203,
            "text": "Get campaign negative keyword example 2",
            "status": "ACTIVE",
            "matchType": "EXACT",
            "modificationTime": "2024-04-08T17:48:31.984",
            "deleted": false
        },
        {
            "id": 542370644,
            "campaignId": 542370539,
            "adGroupId": 427916203,
            "text": "Get campaign negative keyword example 3",
            "status": "ACTIVE",
            "matchType": "EXACT",
            "modificationTime": "2024-04-08T20:52:59.050",
            "deleted": false
        },
        {
            "id": 542370645,
            "campaignId": 542370539,
            "adGroupId": 427916203,
            "text": "Get campaign negative keyword example 4",
            "status": "ACTIVE",
            "matchType": "BROAD",
            "modificationTime": "2024-04-08T20:52:59.054",
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

Update Campaign Negative Keywords

Updates negative keywords in a campaign.

Delete Campaign Negative Keywords

Deletes negative keywords from a campaign.

