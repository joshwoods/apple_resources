

- Apple Search Ads
-  Get a Campaign 

Web Service Endpoint

# Get a Campaign

Fetches a specific campaign by campaign identifier.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}
```

## Path Parameters

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

## Response Codes

` 200 ``OK`

CampaignResponse

`OK`

If the call succeeds, the API returns the Campaign object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to return data for a specific campaign. You can also use a partial fetch as necessary. For more information, see the Use a Partial Fetch section of Using Apple Search Ads API Functionality.

### Payload example: Get a campaign

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/campaigns/{campaignId}
```

```
{
        "id": 542370642,
        "orgId": 40669820,
        "name": "TripTrek campaign 1",
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
        "startTime": "2024-04-08T10:33:31.650",
        "endTime": "2024-04-09T10:33:31.650",
        "status": "ENABLED",
        "servingStatus": "NOT_RUNNING",
        "servingStateReasons": [
            "CAMPAIGN_END_DATE_REACHED"
        ],
        "modificationTime": "2024-04-08T11:00:06.513",
        "deleted": false,
        "sapinLawResponse": "NOT_ANSWERED",
        "countriesOrRegions": [
            "AU",
            "CA",
            "GB",
            "US"
        ],
        "countryOrRegionServingStateReasons": {},
        "billingEvent": "TAPS",
        "supplySources": [
           "APPSTORE_SEARCH_RESULTS"
            ],
        "adChannelType": "SEARCH"
}
```

## See Also

### Campaign Endpoints

Create a Campaign

Creates a campaign to promote an app.

Find Campaigns

Fetches campaigns with selector operators.

Get all Campaigns

Fetches all of an organization’s assigned campaigns.

Update a Campaign

Updates a campaign with a campaign identifier.

Delete a Campaign

Deletes a specific campaign by campaign identifier.

