

- Apple Search Ads
-  Get All Ads 

Web Service Endpoint

# Get All Ads

Fetches all ads assigned to an ad group.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/ads
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

## Response Codes

` 200 ``OK`

AdListResponse

`OK`

If the call succeeds, the API returns the AdListResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to fetch all `ads` assigned to an ad group.

### Payload example: Get all ads

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/ads
```

```
{
    "id": 573408745,
    "orgId": 39872140,
    "campaignId": 570798765,
    "adGroupId": 570798765,
    "creativeId": 94895512,
    "name": "Trip Trek custom product page variation",
    "creativeType": "CUSTOM_PRODUCT_PAGE",
    "status": "PAUSED",
    "servingStatus": "NOT_RUNNING",
    "servingStateReasons": [
      "PAUSED_BY_USER"
      ],
    "deleted": false,
    "creationTime": "2024-10-08T00:18:37.606Z",
    "modificationTime": "2024-10-09T00:18:37.606Z"
}
```

## See Also

### Ad Endpoints

Create an Ad

Creates an ad in an ad group with a creative.

Find Ads

Finds ads within a campaign by selector criteria.

Find Ads (org-level)

Fetches ads within an organization by selector criteria.

Get an Ad

Fetches an ad assigned to an ad group by identifier.

Update an Ad

Updates an ad in an ad group.

Delete an Ad

Deletes an ad from an ad group.

