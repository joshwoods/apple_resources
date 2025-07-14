

- Apple Search Ads
-  Get all Ad Groups 

Web Service Endpoint

# Get all Ad Groups

Fetches all ad groups with a campaign identifier.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups
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

AdGroupListResponse

`OK`

If the call succeeds, the API returns the AdGroup object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

To return all ad groups, use the associated `campaignId` and `adgroupId` in the URI path. You can also use a partial fetch. For more information, see the Use a Partial Fetch section of Using Apple Search Ads API Functionality.

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

Update an Ad Group

Updates an ad group with an ad group identifier.

Delete an Ad Group

Deletes an ad group with a campaign and ad group identifier.

