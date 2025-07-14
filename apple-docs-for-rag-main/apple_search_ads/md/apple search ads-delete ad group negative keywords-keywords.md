

- Apple Search Ads
-  Delete Ad Group Negative Keywords 

Web Service Endpoint

# Delete Ad Group Negative Keywords

Deletes negative keywords from an ad group.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/negativekeywords/delete/bulk
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

`[int64]`

The request body with negative jkeyword IDs.

Content-Type: application/json

## Response Codes

` 200 ``OK`

IntegerResponse

`OK`

If the call succeeds, the API returns the IntegerResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

To delete ad group negative keywords, include the associated `campaignId` and `adgroupId` in the URI. This is a soft deletion.

### Payload example: Delete ad group negative keywords

- Request
- Response

```
POST https://api.searchads.apple.com/api/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/negativekeywords/delete/bulk

[
    578054687,
    578054686,
    578054685
]
```

```
{
    "data": 3,
    "pagination": null,
    "error": null
}
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

Update Ad Group Negative Keywords

Updates negative keywords in an ad group.

