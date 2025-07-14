

- Apple Search Ads
-  Create a Campaign 

Web Service Endpoint

# Create a Campaign

Creates a campaign to promote an app.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/campaigns
```

## HTTP Body

Campaign

The request body that includes the details of the campaign.

Content-Type: application/json

## Response Codes

` 200 ``OK`

CampaignResponse

`OK`

If the call succeeds, the API returns the Campaign object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Apple Search Ads Campaign Management API 3

Apple Search Ads Campaign Management API 4

## Discussion

Essential points for creating campaigns are:

- Use Search for iOS apps to retrieve your `adamId` to use in the request payload.

- Use Find App Eligibility Records to determine your app eligibility to run in campaigns.

- A `dailyBudgetAmount` is a required field to manage the daily budget of your campaigns. Use an optional `budgetAmount` to manage your lifetime budget.

- Use the `countriesOrRegions` attribute to assign App Store locations. To advertise in multiple markets, group countries and regions into a single campaign using ISO alpha-2 country code values.

- See the Campaign object and SupplySource for descriptions of attributes.

After creating a campaign, set up Ad Groups.

### Payload example: Create a campaign

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/campaigns

{
    "orgId": 39879640,
    "name": "TripTrek example campaign",
    "startTime": "2024-05-08T17:00:00.000",
    "endTime": "2024-05-09T17:00:00.000",
    "billingEvent": "TAPS",
    "budgetAmount": {
      "amount": "1500.00",
      "currency": "USD"
    },
    "dailyBudgetAmount": {
      "amount": "250.00",
      "currency": "USD"
    },
    "adamId": 1004806037,
    "countriesOrRegions": ["US","CA"],
    "status": "ENABLED",
    "supplySources": ["APPSTORE_TODAY_TAB"],
    "adChannelType": "DISPLAY"
}
```

```
{
    "data": {
        "id": 585885088,
        "orgId": 39879640,
        "name": "TripTrek Campaign",
        "budgetAmount": {
            "amount": "1500",
            "currency": "USD"
        },
        "dailyBudgetAmount": {
            "amount": "250",
            "currency": "USD"
        },
        "adamId": 1004806037,
        "paymentModel": PAYG,
        "locInvoiceDetails": null,
        "budgetOrders": [],
        "startTime": "2024-05-08T17:00:00.000",
        "endTime": "2024-05-09T17:00:00.000",
        "status": "ENABLED",
        "servingStatus": "NOT_RUNNING",
        "creationTime": "2024-05-04T20:15:04.382",
        "servingStateReasons": [
            "APP_NOT_PUBLISHED_YET",
            "CAMPAIGN_START_DATE_IN_FUTURE",
            "AD_GROUP_MISSING"
        ],
        "modificationTime": "2024-05-04T20:15:04.747",
        "deleted": false,
        "sapinLawResponse": "NOT_ANSWERED",
        "countriesOrRegions": [
            "CA",
            "US"
        ],
        "countryOrRegionServingStateReasons": {
            "CA": [
                "APP_NOT_PUBLISHED_YET"
            ],
            "US": [
                "APP_NOT_PUBLISHED_YET"
            ]
        },
        "supplySources": [
            "APPSTORE_TODAY_TAB"
        ],
        "adChannelType": "DISPLAY",
        "billingEvent": "TAPS",
        "displayStatus": "ON_HOLD"
    },
    "pagination": null,
    "error": null
}
```

## See Also

### Campaign Endpoints

Find Campaigns

Fetches campaigns with selector operators.

Get a Campaign

Fetches a specific campaign by campaign identifier.

Get all Campaigns

Fetches all of an organization’s assigned campaigns.

Update a Campaign

Updates a campaign with a campaign identifier.

Delete a Campaign

Deletes a specific campaign by campaign identifier.

