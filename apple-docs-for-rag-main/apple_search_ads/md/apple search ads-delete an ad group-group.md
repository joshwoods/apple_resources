

- Apple Search Ads
-  Delete an Ad Group 

Web Service Endpoint

# Delete an Ad Group

Deletes an ad group with a campaign and ad group identifier.

Search Ads 5.0+

## URL

``` source
DELETE https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}
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

VoidResponse

`OK`

If the call succeeds, the API returns the AdGroup object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

## See Also

### Ad Group Endpoints

Create an Ad Group

Creates an ad group as part of a campaign.

Find Ad Groups

Fetches ad groups within a campaign.

Find Ad Groups (org-level)

Fetches ad groups within an organization.

Get an Ad Group

Fetches a specific ad group with a campaign and ad group identifier.

Get all Ad Groups

Fetches all ad groups with a campaign identifier.

Update an Ad Group

Updates an ad group with an ad group identifier.

