

- Apple Search Ads
-  Find Campaigns 

Web Service Endpoint

# Find Campaigns

Fetches campaigns with selector operators.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns/find
```

## HTTP Body

Selector

The request body that includes the selector Condition. Selector objects define what data the API returns when fetching resources.

Content-Type: application/json

## Response Codes

` 200 ``OK`

CampaignListResponse

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

## Discussion

Use this endpoint to find campaigns using a Selector Condition to narrow results. If you don’t specify selector conditions, all campaign objects return in the response. See the Campaign object for parameter descriptions and selector condition operators.

### Payload example: Find campaigns

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns/find

{
    "pagination": { 
        "offset": 0,
        "limit": 1000
    },
    "orderBy": [
        {
            "field": "id",
            "sortOrder": "ASCENDING"
        }
    ],
    "conditions": [
        {
            "field": "countriesOrRegions",
            "operator": "CONTAINS_ALL",
            "values": [
                "US","CA"
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
      "orgId": 40669820,
      "name": "TripTrek example campaign",
      "budgetAmount": {
        "amount": "2000",
        "currency": "USD"
      },
      "dailyBudgetAmount": {
        "amount": "500",
        "currency": "USD"
      },
      "adamId": 427916203,
      "paymentModel": "PAYG",
      "locInvoiceDetails": null,
      "budgetOrders": [],
      "displayStatus": "ON_HOLD",
      "adChannelType": "SEARCH",
      "supplySources": [
        "APPSTORE_SEARCH_RESULTS"
      ],
      "billingEvent": "TAPS",
      "startTime": "2024-04-08T10:33:31.650",
      "endTime": "2024-04-09T10:33:31.650",
      "status": "ENABLED",
      "servingStatus": "AD_GROUP_MISSING",
      "servingStateReasons": [
        "CAMPAIGN_START_DATE_IN_FUTURE"
      ],
      "modificationTime": "2024-04-08T23:58:05.316",
      "deleted": false,
      "sapinLawResponse": "NOT_ANSWERED",
      "countriesOrRegions": [
        "CA",
        "JP",
        "NZ",
        "US"
      ],
      "countryOrRegionServingStateReasons": {}
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

### Campaign Endpoints

Create a Campaign

Creates a campaign to promote an app.

Get a Campaign

Fetches a specific campaign by campaign identifier.

Get all Campaigns

Fetches all of an organization’s assigned campaigns.

Update a Campaign

Updates a campaign with a campaign identifier.

Delete a Campaign

Deletes a specific campaign by campaign identifier.

