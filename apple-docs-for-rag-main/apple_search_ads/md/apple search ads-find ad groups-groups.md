

- Apple Search Ads
-  Find Ad Groups 

Web Service Endpoint

# Find Ad Groups

Fetches ad groups within a campaign.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/{campaignId}/adgroups/find
```

## Path Parameters

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

## HTTP Body

Selector

The request body that includes the selector Condition. Selector objects define what data the API returns when fetching resources.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AdGroupListResponse

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

## Mentioned in 

Apple Search Ads Campaign Management API 5

## Discussion

Use this endpoint to find ad groups within campaigns using the associated `campaignId` in the resource path. Use a Selector Condition to narrow results. If you don’t specify selector conditions, all ad groups in campaigns return. See the AdGroup object for field descriptions and selector condition operators.

### Payload example: Find ad groups

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns//adgroups/find

{
  "pagination": {
    "offset": 0,
    "limit": 20
  },
  "fields": null,
  "orderBy": [
    {
      "field": "id",
      "sortOrder": "ASCENDING"
    }
  ],
  "conditions": [
    {
      "field": "pricingModel",
      "operator": "EQUALS",
      "values": [
        "CPC"
      ]
    }
  ]
}
```

```
{
  "data": [
    {
      "id": 542370642,
      "campaignId": 56543219,
      "name": "Trip Trek ad group 1",
      "cpaGoal": null,
      "startTime": "2024-04-08T07:00:00.000",
      "endTime": null,
      "automatedKeywordsOptIn": true,
      "defaultBidAmount": {
        "amount": "1",
        "currency": "USD"
      },
      "pricingModel": "CPC",
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
        "appDownloaders": {
          "included": [],
          "excluded": []
        }
      },
      "orgId": 40669820,
      "modificationTime": "2024-04-08T23:30:17.280",
      "status": "ENABLED",
      "servingStatus": "RUNNING",
      "servingStateReasons": null,
      "displayStatus": "RUNNING",
      "deleted": false
    },
    {
      "id": 542370643,
      "campaignId": 56543219,
      "name": "Trip Trek ad group 2",
      "cpaGoal": null,
      "startTime": "2024-04-08T23:46:00.000",
      "endTime": "2024-04-09T05:00:00.000",
      "automatedKeywordsOptIn": true,
      "defaultCpcBid": {
        "amount": "1",
        "currency": "USD"
      },
      "pricingModel": "CPC",
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
        "appDownloaders": {
          "included": [],
          "excluded": []
        }
      },
      "orgId": 40669820,
      "modificationTime": "2024-04-08T05:15:36.518",
      "status": "ENABLED",
      "servingStatus": "RUNNING",
      "servingStateReasons": [
        "null"
      ],
      "displayStatus": "RUNNING",
      "deleted": false
    },
    {
      "id": 542370644,
      "campaignId": 56543219,
      "name": "Trip Trek ad group 3",
      "cpaGoal": null,
      "startTime": "2024-04-08T23:45:00.000",
      "endTime": "2024-04-09T06:59:00.000",
      "automatedKeywordsOptIn": true,
      "defaultBidAmount": {
        "amount": "100",
        "currency": "USD"
      },
      "pricingModel": "CPC",
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
        "appDownloaders": {
          "included": [],
          "excluded": []
        }
      },
      "orgId": 40669820,
      "modificationTime": "2024-04-08T07:15:21.110",
      "status": "ENABLED",
      "servingStatus": "NOT_RUNNING",
      "servingStateReasons": [
        "ADGROUP_END_DATE_REACHED"
      ],
      "displayStatus": "ON_HOLD",
      "deleted": false
    },
    {
      "id": 542370645,
      "campaignId": 56543219,
      "name": "Trip Trek ad group 4",
      "cpaGoal": {
        "amount": "100",
        "currency": "USD"
      },
      "startTime": "2024-04-08T19:10:31.650",
      "endTime": "2024-04-09T19:33:31.650",
      "automatedKeywordsOptIn": false,
      "defaultBidAmount": {
        "amount": "1",
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
        "daypart": {
          "userTime": {
            "included": [
              1,
              3,
              22,
              24
            ]
          }
        },
        "appDownloaders": null
      },
      "orgId": 40669820,
      "modificationTime": "2024-04-08T18:06:20.305",
      "status": "ENABLED",
      "servingStatus": "RUNNING",
      "servingStateReasons": null,
      "displayStatus": "RUNNING",
      "deleted": false
    }
  ],
  "pagination": {
    "totalResults": 4,
    "startIndex": 1,
    "itemsPerPage": 10
  }
}
```

## See Also

### Ad Group Endpoints

Create an Ad Group

Creates an ad group as part of a campaign.

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

