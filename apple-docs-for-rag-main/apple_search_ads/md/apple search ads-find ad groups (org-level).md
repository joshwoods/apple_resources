

- Apple Search Ads
-  Find Ad Groups (org-level) 

Web Service Endpoint

# Find Ad Groups (org-level)

Fetches ad groups within an organization.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/adgroups/find
```

## HTTP Body

Selector

The request body that includes the selector Condition. Selector objects define what data the API returns when fetching resources.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AdGroupListResponse

`OK`

Use this endpoint to find ad groups within your organization. Use a Selector Condition to narrow results. If you don’t specify selector conditions, all of your ad groups return in the API response. See the AdGroup object for field descriptions and selector condition operators.

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

Use this endpoint to find ad groups within your organization. Use a Selector Condition to narrow results. If you don’t specify selector conditions, all of your ad groups return in the API response. See the AdGroup object for field descriptions and selector condition operators.

### Payload example: Find ad groups (org-level)

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/adgroups/find

{
  "fields": null,
  "conditions": [
    {
      "field": "pricingModel",
      "operator": "EQUALS",
      "values": [
        "CPC"
      ]
    }
  ],
  "orderBy": [
    {
      "field": "id",
      "sortOrder": "ASCENDING"
    }
  ],
  "pagination": {
    "offset": 0,
    "limit": 20
  }
}

```

```
{
  "data": [
    {
      "id": 542370764,
      "campaignId": 56543219,
      "name": "Trip Trek ad group 5",
      "cpaGoal": null,
      "paymentModel": "PAYG",
      "startTime": "2024-10-20T20:37:21.146Z",
      "endTime": "2024-10-20T20:37:21.146Z",
      "automatedKeywordsOptIn": true,
      "defaultBidAmount": {
        "amount": "1",
        "currency": "USD"
      },
      "pricingModel": "CPC",
      "targetingDimensions": {
        "age": {
          "included": [
            {
              "minAge": 18,
              "maxAge": 55
            }
          ]
        },
        "gender": {
          "included": [
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
            "CA"
          ]
        },
        "locality": {
          "included": [
            "Cupertino"
          ]
        },
        "deviceClass": {
          "included": [
            "IPHONE",
            "IPAD"
          ]
        },
        "daypart": {
          "userTime": {
            "included": [
              0
            ]
          }
        },
        "appDownloaders": {
          "included": [
            "654327167"
          ],
          "excluded": [
            "654325422"
          ]
        },
        "appCategories": {
          "included": [
            100
          ],
          "excluded": [
            100
          ]
        }
      },
      "orgId": 40669876,
      "modificationTime": "2024-10-20T20:37:21.146Z",
      "status": "ENABLED",
      "servingStatus": "RUNNING",
      "servingStateReasons": [
        "null"
      ],
      "displayStatus": "RUNNING",
      "deleted": false
    }
  ],
  "pagination": {
    "totalResults": 1,
    "startIndex": 1,
    "itemsPerPage": 10
  }
}
```

## See Also

### Ad Group Endpoints

Create an Ad Group

Creates an ad group as part of a campaign.

Find Ad Groups

Fetches ad groups within a campaign.

Get an Ad Group

Fetches a specific ad group with a campaign and ad group identifier.

Get all Ad Groups

Fetches all ad groups with a campaign identifier.

Update an Ad Group

Updates an ad group with an ad group identifier.

Delete an Ad Group

Deletes an ad group with a campaign and ad group identifier.

