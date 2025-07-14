

- Apple Search Ads
-  Delete a Campaign 

Web Service Endpoint

# Delete a Campaign

Deletes a specific campaign by campaign identifier.

Search Ads 5.0+

## URL

``` source
DELETE https://api.searchads.apple.com/api/v5/campaigns/{campaignId}
```

## Path Parameters

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

## Response Codes

` 200 ``OK`

VoidResponse

`OK`

If the call succeeds, the API returns the Campaign objects in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

### Campaign Endpoints

Create a Campaign

Creates a campaign to promote an app.

Find Campaigns

Fetches campaigns with selector operators.

Get a Campaign

Fetches a specific campaign by campaign identifier.

Get all Campaigns

Fetches all of an organization’s assigned campaigns.

Update a Campaign

Updates a campaign with a campaign identifier.

