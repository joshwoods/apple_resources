

- Apple Search Ads
-  Get all Campaigns 

Web Service Endpoint

# Get all Campaigns

Fetches all of an organization’s assigned campaigns.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/campaigns
```

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

CampaignListResponse

`OK`

If the call succeeds, the API returns a list of Campaign objects in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

This endpoint returns data for all of an organization’s assigned campaigns. You can also use a partial fetch as necessary. For more information, see the Use a Partial Fetch section of Using Apple Search Ads API Functionality.

## See Also

### Campaign Endpoints

Create a Campaign

Creates a campaign to promote an app.

Find Campaigns

Fetches campaigns with selector operators.

Get a Campaign

Fetches a specific campaign by campaign identifier.

Update a Campaign

Updates a campaign with a campaign identifier.

Delete a Campaign

Deletes a specific campaign by campaign identifier.

