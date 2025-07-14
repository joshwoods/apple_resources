

- Apple Search Ads
-  Update a Campaign 

Web Service Endpoint

# Update a Campaign

Updates a campaign with a campaign identifier.

Search Ads 5.0+

## URL

``` source
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}
```

## Path Parameters

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

## HTTP Body

UpdateCampaignRequest

The request body that includes the details of the campaign.

Content-Type: application/json

## Response Codes

` 200 ``OK`

CampaignResponse

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

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

Use this endpoint to update countries or regions (App Store geolocations) where you promote your app, and to set your campaign budget. Use the associated `campaignId` in the URI.

To edit a subset of object properties without having to include all object properties in the payload, use partial updates. Use a campaign object envelope in your campaign update request payloads. Other objects don’t require a JSON envelope. See the Use Partial Updates section of Using Apple Search Ads API Functionality.

### Payload example: Update a campaign

- Request
- Response

```
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}

{
  "clearGeoTargetingOnCountryOrRegionChange": true,
  "campaign": {
    "name”: “TripTrek campaign 1",
    "budgetAmount": {
      "amount": "2000",
      "currency": "USD"
    },
    "dailyBudgetAmount": {
      "amount": "250",
      "currency": "USD"
    },
    "budgetOrders": [
      0
    ],
    "locInvoiceDetails": {
      "clientName": "client name",
      "orderNumber": "7565239",
      "primaryBuyerName": "buyer name",
      "primaryBuyerEmail": "buyer email",
      "billingContactEmail": "billing email"
    },
    "status": "ENABLED",
    "countriesOrRegions": [
      "US",
      "CA",
      "GB",
      "AU"
    ]
  }
}
```

```
{
  "id": 542370539,
  "orgId": 40669820,
  "name": "TripTrek campaign 1",
  "budgetAmount": {
    "amount": "2000",
    "currency": "USD"
  },
  "dailyBudgetAmount": {
    "amount": "250",
    "currency": "USD"
  },
  "adamId": 422689480,
  "paymentModel": “PAYG”,
  "billingEvent": "TAPS",
  "locInvoiceDetails": {
    "clientName": "client name",
    "orderNumber": "7565239",
    "buyerName": "buyer name",
    "buyerEmail": "buyer email",
    "billingContactEmail": "billing e-mail"
  },
  "budgetOrders": [
    34562211,
    34562212
  ],
  "supplySources": [
    "APPSTORE_SEARCH_RESULTS"
  ],
  "adChannelType": "SEARCH",
  "displayStatus": "RUNNING",
  "startTime": "2024-05-18T12:00:00.000Z",
  "endTime": "2024-05-22T12:00:00.000Z",
  "status": "ENABLED",
  "servingStatus": "RUNNING",
  "servingStateReasons": [
    [
      "null"
    ]
  ],
  "modificationTime": "2024-05-09T17:20:33.919Z",
  "deleted": false,
  "countriesOrRegions": [
    "AU",
    "CA",
    "GB",
    "US"
  ],
  "countryOrRegionServingStateReasons": {
  }
}
```

### Payload example: Update a campaign budget amount or daily budget amount

- Request
- Response

```
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}

{
  "campaign": {
    "budgetAmount": null,
    "dailyBudgetAmount": {
      "amount": "300",
      "currency": "USD"
    }
  }
}
```

```
{
  "data": {
    "id": 586640439,
    "orgId": 39879640,
    "name": "TripTrek campaign",
    "budgetAmount": null,
    "dailyBudgetAmount": {
      "amount": "300",
      "currency": "USD"
    },
    "adamId": 1004806037,
    "paymentModel": "PAYG",
    "locInvoiceDetails": null,
    "budgetOrders": [],
    "startTime": "2024-05-18T17:00:00.000",
    "endTime": "2024-05-22T17:00:00.000",
    "status": "ENABLED",
    "servingStatus": "NOT_RUNNING",
    "creationTime": "2024-05-11T19:59:51.484",
    "servingStateReasons": [
      "CAMPAIGN_START_DATE_IN_FUTURE",
      "AD_GROUP_MISSING"
    ],
    "modificationTime": "2024-05-11T20:08:40.809",
    "deleted": false,
    "sapinLawResponse": "NOT_ANSWERED",
    "countriesOrRegions": [
      "US"
    ],
    "supplySources": [
      "APPSTORE_SEARCH_TAB"
    ],
    "adChannelType": "DISPLAY",
    "billingEvent": "TAPS",
    "displayStatus": "ON_HOLD"
  },
  "pagination": null,
  "error": null
}
```

### Payload example: Update a campaign with countries or regions

- Request
- Response

```
PUT https://api.searchads.apple.com/api/v5/campaigns/{campaignId}

{
  "clearGeoTargetingOnCountryOrRegionChange": true,
  "campaign": {
    "countriesOrRegions": [
      "US",
      "CA",
      "GB",
      "AU"
    ]
  }
}
```

```
{
  "id": 542370642,
  "orgId": 40669820,
  "name": "TripTrek campaign 2",
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
  "billingEvent": "TAPS",
  "supplySources": [
    "APPSTORE_SEARCH_RESULTS"
  ],
  "adChannelType": "SEARCH",
  "displayStatus": "RUNNING",
  "startTime": "2024-05-18T00:00:00.000",
  "endTime": "2024-05-22T00:00:00.000",
  "status": "ENABLED",
  "servingStatus": "RUNNING",
  "servingStateReasons": null,
  "modificationTime": "2024-05-08T18:27:56.380",
  "deleted": false,
  "sapinLawResponse": "NOT_ANSWERED",
  "countriesOrRegions": [
    "AU",
    "CA",
    "GB",
    "US"
  ],
  "countryOrRegionServingStateReasons": {}
}
```

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

Delete a Campaign

Deletes a specific campaign by campaign identifier.

