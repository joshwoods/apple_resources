

- Apple Search Ads
-  Get an Ad Group Negative Keyword 

Web Service Endpoint

# Get an Ad Group Negative Keyword

Fetches a specific negative keyword in an ad group.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/negativekeywords/{keywordId}
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

NegativeKeywordResponse

`OK`

If the call succeeds, the API returns the NegativeKeywordResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

To return a specific negative keyword, use the associated `campaignId`, `adgroupId`, and `keywordId` in the URI. You can also use a partial fetch. For more information, see the Use a Partial Fetch section of Using Apple Search Ads API Functionality.

### Payload example: Get an ad group negative keyword

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/negativekeywords/{keywordId}
```

```
{
  "id": 542370642,
  "campaignId": 542370539,
  "adGroupId": 427916203,
  "text": "ad group negative keyword example 1",
  "status": "ACTIVE",
  "matchType": "EXACT",
  "modificationTime": "2024-04-08T17:49:30.399",
  "deleted": false
}
```

## See Also

### Ad Group Negative Keywords Endpoints

Create Ad Group Negative Keywords

Creates negative keywords in a specific ad group.

Find Ad Group Negative Keywords

Fetches negative keywords in a campaign’s ad groups.

Get All Ad Group Negative Keywords

Fetches all negative keywords in ad groups.

Update Ad Group Negative Keywords

Updates negative keywords in an ad group.

Delete Ad Group Negative Keywords

Deletes negative keywords from an ad group.

