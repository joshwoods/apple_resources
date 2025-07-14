

- Apple Search Ads
-  Get an Ad Group 

Web Service Endpoint

# Get an Ad Group

Fetches a specific ad group with a campaign and ad group identifier.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}
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

AdGroupResponse

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

To return a specific ad group, use the associated `campaignId` and `adgroupId` in the URI path. You can also use a partial fetch. For more information, see the Use a Partial Fetch subsection of Using Apple Search Ads API Functionality.

### Payload example: Get an ad group

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}
```

```
{
    "id": 542370539,
    "campaignId": 56543219,
    "name": " ad group name example",
    "cpaGoal": {
      "amount": "100",
      "currency": "USD"
    },
    "startTime": "2024-04-08T12:00:22.788",
    "endTime": "2024-04-09T12:00:22.788",
    "automatedKeywordsOptIn": false,
    "defaultBidAmount": {
      "amount": "100",
      "currency": "USD"
    },
   "pricingModel": "CPC",    
   "targetingDimensions": {
      "age": {
        "included": [
          {
            "minAge": 20,
            "maxAge": 25
          },
          {
            "minAge": 25,
            "maxAge": 55
          }
        ]
      },
      "gender": {
        "included": [
          "M",
          "F"
        ]
      },
      "country": null,
      "adminArea": null,
      "locality": null,
      "deviceClass": {
        "included": [
          "IPAD",
          "IPHONE"
        ]
      },
      "daypart": {
        "userTime": {
          "included": [
            1,
            3,
            22
          ]
        }
      },
      "appDownloaders": null
    },
    "orgId": 40669820,
    "modificationTime": "2024-04-08T19:00:24.105",
    "status": "ENABLED",
    "servingStatus": "RUNNING",
    "servingStateReasons": null,
    "displayStatus": "RUNNING",
    "deleted": false
}
```

## See Also

### Ad Group Endpoints

Create an Ad Group

Creates an ad group as part of a campaign.

Find Ad Groups

Fetches ad groups within a campaign.

Find Ad Groups (org-level)

Fetches ad groups within an organization.

Get all Ad Groups

Fetches all ad groups with a campaign identifier.

Update an Ad Group

Updates an ad group with an ad group identifier.

Delete an Ad Group

Deletes an ad group with a campaign and ad group identifier.

