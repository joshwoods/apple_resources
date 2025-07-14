

- Apple Search Ads
-  Get a Campaign Negative Keyword 

Web Service Endpoint

# Get a Campaign Negative Keyword

Fetches a specific negative keyword in a campaign.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/negativekeywords/{keywordId}
```

## Path Parameters

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

NegativeKeywordResponse

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

To return a specific campaign negative keyword, use the associated `campaignId` and `keywordId` in the URI. You can also use a partial fetch. For more information, see the Use a Partial Fetch section of Using Apple Search Ads API Functionality.

### Payload example: Get a campaign negative keyword

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/negativekeywords/{keywordId}
```

```
{  
  "id": 542370642,
  "campaignId": 542370539,
  "adGroupId": 542317095,
  "text": "Get campaign negative keywords example",
  "status": "ACTIVE",
  "matchType": "BROAD",
  "modificationTime": "2024-04-08T17:48:31.979",
  "deleted": false
}

```

## See Also

### Campaign Negative Keywords Endpoints

Create Campaign Negative Keywords

Creates negative keywords for a campaign.

Find Campaign Negative Keywords

Fetches negative keywords for campaigns.

Get All Campaign Negative Keywords

Fetches all negative keywords in a campaign.

Update Campaign Negative Keywords

Updates negative keywords in a campaign.

Delete Campaign Negative Keywords

Deletes negative keywords from a campaign.

