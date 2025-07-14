

- Apple Search Ads
-  Get a Targeting Keyword in an Ad Group 

Web Service Endpoint

# Get a Targeting Keyword in an Ad Group

Fetches a specific targeting keyword in an ad group.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/targetingkeywords/{keywordId}
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

`keywordId`

`int64`

 (Required) 

The unique identifier for the keyword.

## Response Codes

` 200 ``OK`

KeywordResponse

`OK`

If the call succeeds, the API returns the Keyword object in the response payload with an HTTP status code of `200` `(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

To return a specific targeting keyword, use the associated `campaignId`, `adgroupId`, and `keywordId` in the URI. You can also use a partial fetch. For more information, see the Use a Partial Fetch section of Using Apple Search Ads API Functionality.

### Payload example: Get a targeting keyword in an ad group

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/targetingkeywords/{keywordId}
```

```
{  
  "id": 542370642,
  "adGroupId": 427916203,
  "text": "targeting keyword example 1",
  "status": "ACTIVE",
  "matchType": "BROAD",
  "bidAmount": {
    "amount": "100",
    "currency": "USD"
  },
  "modificationTime": "2024-04-08T20:48:28.206",
  "deleted": false
}
```

## See Also

### Ad Group Targeting Keywords Endpoints

Create Targeting Keywords

Creates targeting keywords in ad groups.

Find Targeting Keywords in a Campaign

Fetches targeting keywords in a campaign’s ad groups.

Get All Targeting Keywords in an Ad Group

Fetches all targeting keywords in ad groups.

Update Targeting Keywords

Updates targeting keywords in ad groups.

Delete Targeting Keywords

Deletes targeting keywords from ad groups.

Delete a Targeting Keyword

Deletes a targeting keyword in an ad group.

