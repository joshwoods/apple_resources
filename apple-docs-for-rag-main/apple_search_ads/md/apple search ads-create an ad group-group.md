

- Apple Search Ads
-  Create an Ad Group 

Web Service Endpoint

# Create an Ad Group

Creates an ad group as part of a campaign.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups
```

## Path Parameters

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

## HTTP Body

AdGroup

The request body that includes the details of the ad group and campaign.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AdGroupResponse

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

## Discussion

To create ad groups, use the associated `campaignId` as a resource in the URI. In the request, specify TargetingDimensions and apply it to ad groups.

Note

You can’t create or update ad groups with geotargeting for campaigns with multiple `countriesOrRegions`.

### Payload example: Create an ad group with targeting

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups

{
  "campaignId": 56543219,
  "name": "TripTrek ad group",
  "cpaGoal": {
    "amount": "1",
    "currency": "USD"
  },
  "startTime": "2024-05-18T00:00:00.000",
  "endTime": "2024-05-22T00:00:00.000",
  "automatedKeywordsOptIn": true,
  "pricingModel": "CPC",
  "defaultBidAmount": {
    "amount": "1",
    "currency": "USD"
  },
 "targetingDimensions": {
    "age": {
      "included": [
        {
          "minAge": 20,
          "maxAge": 25
        }
      ]
    },
    "gender": {
      "included": [
        "F",
        "M"
      ]
    },
    "deviceClass": {
      "included": [
        "IPAD",
        "IPHONE"
        ]
    }
  },
  "orgId": 39879640,
  "status": "ENABLED"
}
```

```
{
  "id": 542370642,
  "campaignId": 56543219,
  "name": "TripTrek ad group",
  "cpaGoal": {
    "amount": "1",
    "currency": "USD"
  },
  "startTime": "2024-05-18T00:00:00.000",
  "endTime": "2024-05-22T00:00:00.000",
  "automatedKeywordsOptIn": true,
  "pricingModel": "CPC",
  "defaultBidAmount": {
    "amount": "1",
    "currency": "USD"
  },
  "targetingDimensions": {
    "age": {
      "included": [
        {
          "minAge": 20,
          "maxAge": 25
        }
      ]
    },
    "gender": {
      "included": [
        "F",
        "M"
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
    "appDownloaders": null
  },
  "orgId": 40669820,
  "modificationTime": "2024-05-22T17:30:56.435",
  "status": "ENABLED",
  "servingStatus": "NOT_RUNNING",
  "servingStateReasons": [
    "START_DATE_IN_THE_FUTURE"
  ],
  "displayStatus": "ON_HOLD",
  "deleted": false
}
```

### Payload example: Create an ad group without targeting

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups

{
  "name": "TripTrek ad group",
  "startTime": "2024-05-18T00:00:00.000",
  "endTime": "2024-05-22T00:00:00.000",
  "automatedKeywordsOptIn": false,
  "pricingModel": "CPC",
  "defaultBidAmount": {
    "amount": "1",
    "currency": "USD"
  },
  "orgId": 39879640,
  "status": "ENABLED"
}
```

```
{
  "data": {
    "id": 586648342,
    "campaignId": 586640439,
    "name": "TripTrek ad group",
    "cpaGoal": null,
    "startTime": "2024-05-18T00:00:00.000",
    "endTime": "2024-05-22T00:00:00.000",
    "automatedKeywordsOptIn": false,
    "targetingDimensions": {
      "age": null,
      "gender": null,
      "country": null,
      "adminArea": null,
      "locality": null,
      "deviceClass": {
        "included": [
          "IPHONE",
          "IPAD"
        ]
      },
      "daypart": null,
      "appDownloaders": null
    },
    "orgId": 39879640,
    "creationTime": "2024-05-11T20:22:04.405",
    "pricingModel": "CPC",
    "modificationTime": "2024-05-11T20:22:04.405",
    "status": "ENABLED",
    "servingStatus": "NOT_RUNNING",
    "servingStateReasons": [
      "START_DATE_IN_THE_FUTURE"
    ],
    "displayStatus": "ON_HOLD",
    "deleted": false,
    "defaultBidAmount": {
      "amount": "1",
      "currency": "USD"
    }
  },
  "pagination": null,
  "error": null
}
```

## See Also

### Ad Group Endpoints

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

Delete an Ad Group

Deletes an ad group with a campaign and ad group identifier.

