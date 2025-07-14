

- Apple Search Ads
-  Update an Ad Group 

Web Service Endpoint

# Update an Ad Group

Updates an ad group with an ad group identifier.

Search Ads 5.0+

## URL

``` source
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}
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

AdGroupUpdate

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

To update ad groups, use the associated `campaignId` and `adgroupId` in the resource path.

In the request, specify TargetingDimensions and apply it to ad groups. If you’re not updating TargetingDimensions, don’t include them in the payload. Use partial updates as necessary. For more information, see the Use Partial Updates section of Using Apple Search Ads API Functionality.

Note

You can’t create or update ad groups with geotargeting for campaigns with multiple countries or regions. Use UpdateCampaignRequest to clear your geotargeting parameters. Then apply TargetingDimensions in the request payload.

### Payload example: Update an ad group with targeting

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups 

{
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
    "country": {
      "included": [
        "US"
      ]
    },
    "adminArea": {
      "included": [
        "US|CA"
      ]
    },
    "locality": {
      "included": [
        "US|CA|Cupertino"
      ]
    },
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
    }
  }
}
```

```
{
  "id": 542370539,
  "campaignId": 542370539,
  "name": "TripTrek ad group 2",
  "cpaGoal": {
    "amount": "100",
    "currency": "USD"
  },
  "startTime": "2024-04-08T16:20:31.650",
  "endTime": "2024-04-09T19:33:31.650",
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
        }
      ]
    },
    "gender": {
      "included": [
        "M",
        "F"
      ]
    },
    "country": {
      "included": [
        "US"
      ]
    },
    "adminArea": {
      "included": [
        "US|CA"
      ]
    },
    "locality": {
      "included": [
        "US|CA|Cupertino"
      ]
    },
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
  "modificationTime": "2024-04-08T17:15:56.956",
  "status": "ENABLED",
  "servingStatus": "NOT_RUNNING",
  "servingStateReasons": [
    "START_DATE_IN_THE_FUTURE"
  ],
  "displayStatus": "ON_HOLD",
  "deleted": false
}
```

### Payload example: Update an ad group without targeting

- Request
- Response

```
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}

{
  "name": "TripTrek AdGroup 2",
  "startTime": "2024-05-08T17:00:00.000"
}

```

```
{
    "data": {
        "id": 585885654,
        "campaignId": 585885088,
        "name": "TripTrek AdGroup 2",
        "cpaGoal": null,
        "startTime": “2024-05-08T17:00:00.000”,
        "endTime": null,
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
        "creationTime": "2024-05-04T20:49:47.286",
        "pricingModel": "CPC",
        "modificationTime": "2023-05-04T20:49:47.286",
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

### Payload example: Update an ad group to show a CPA goal

- Request
- Response

```
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/{adgroupId}

{
  "campaignId": 585885088,
  "name": "TripTrek ad group 3",
  "cpaGoal": {
    "amount": "1",
    "currency": "USD"
  },
  "startTime": "2024-05-08T10:00:00.000",
  "endTime": "2024-05-09T10:00:00.000",
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
        "id": 585887393,
        "campaignId": 585886890,
        "name": "TripTrek ad group 3",
        "cpaGoal": {
            "amount": "1",
            "currency": "USD"
        },
        "startTime": "2024-05-08T10:00:00.000",
        "endTime": "2024-05-09T10:00:00.000",
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
        "creationTime": "2024-05-04T23:33:33.211",
        "pricingModel": "CPC",
        "modificationTime": "2024-05-04T23:33:33.211",
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

Delete an Ad Group

Deletes an ad group with a campaign and ad group identifier.

