

- Apple Search Ads
-  Delete Targeting Keywords 

Web Service Endpoint

# Delete Targeting Keywords

Deletes targeting keywords from ad groups.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/targetingkeywords/delete/bulk
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

The request body.

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

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

To delete ad group keywords, include the associated `campaignId` and `adgroupId` in the URI. This is a soft deletion.

### Payload example: Delete targeting keywords

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/targetingkeywords/delete/bulk

[
    578054698,
    578054665,
    578054632
]
```

```
{
    "data": 2,
    "pagination": null,
    "error": null
}

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

Update Targeting Keywords

Updates targeting keywords in ad groups.

Delete a Targeting Keyword

Deletes a targeting keyword in an ad group.

