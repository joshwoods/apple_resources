

- Apple Search Ads
-  Update an Ad 

Web Service Endpoint

# Update an Ad

Updates an ad in an ad group.

Search Ads 5.0+

## URL

``` source
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/ads/{adId}
```

## Path Parameters

`adId`

`int64`

 (Required) 

A unique identifier representing the assignment relationship between an ad group and an Ad.

`adgroupId`

`int64`

 (Required) 

The unique identifier for the ad group.

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

## HTTP Body

AdUpdate

The request body that includes the details of the Creative.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AdResponse

`OK`

If the call succeeds, the API returns the AdResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to update or replace an Ad. Use your `adId` in the resource path. The follow-up step is to create an Ad using your `creativeId`. See Create an Ad. You can assign one active custom product page to an ad group. For information about how to edit a subset of object properties without having to include all object properties in the payload, see the Use Partial Updates section in Using Apple Search Ads API Functionality.

### Payload example: Update an ad

- Request
- Response

```
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}/ads/{adId}

{
  "name": "Trip Trek custom product page variation",
  "status": "PAUSED"
}
```

```
{
    "id": 573408745,
    "orgId": 39872140,
    "campaignId": 570798765,
    "adGroupId": 427916203,
    "creativeId": 94895512,
    "name": "Trip Trek custom product page variation",
    "creativeType": "CUSTOM_PRODUCT_PAGE",
    "status": "PAUSED",
    "servingStatus": "NOT_RUNNING",
    "servingStateReasons": [
      "PAUSED_BY_USER"
      ],
    "deleted": false,
    "creationTime": "2024-11-16T01:15:32.412Z",
    "modificationTime": "2024-11-16T01:15:32.412Z"
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

Get All Ads

Fetches all ads assigned to an ad group.

Delete an Ad

Deletes an ad from an ad group.

