

- Apple Search Ads
-  Get Campaign-Level Reports 

Web Service Endpoint

# Get Campaign-Level Reports

Fetches reports for campaigns.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/reports/campaigns
```

## HTTP Body

ReportingRequest

The report request body consisting of metrics and dimensions to use as filters.

Content-Type: application/json

## Response Codes

` 200 ``OK`

ReportingResponseBody

`OK`

If the call succeeds, the API returns the ReportingResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to fetch reports for your campaigns. See ReportingCampaign and CampaignAppDetail for Condition operators and field values to filter results with a Selector.

See the `groupBy` parameter description in the ReportingRequest for supported values per targeting dimension.

The `orderBy` Selector specifies fields to sort the records list by `ASCENDING` or `DESCENDING`. All ReportingCampaign fields are available to the `orderBy` Selector except `servingStateReasons`, `app`, `app:{appName}`, and `app:{adamId}`.

### Payload example 1: Get campaign-level reports

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/reports/campaigns

{
  "startTime": "2024-04-08",
  "endTime": "2024-04-09",
  "selector": {
    "orderBy": [
      {
        "field": "countryOrRegion",
        "sortOrder": "ASCENDING"
      }
    ],
    "conditions": [
      {
        "field": "countriesOrRegions",
        "operator": "CONTAINS_ANY",
        "values": [
          "US",
          "GB"
        ]
      },
      {
        "field": "countryOrRegion",
        "operator": "IN",
        "values": [
          "US"
        ]
      }
    ],
    "pagination": {
      "offset": 0,
      "limit": 1000
    }
  },
  "groupBy": [
    "countryOrRegion"
  ],
  "timeZone": "UTC",
  "returnRecordsWithNoMetrics": true,
  "returnRowTotals": true,
  "returnGrandTotals": true
}
```

```
{
    "row": [
      {
        "other": false,
        "granularity": [
          {
            "impressions": 17        
            "taps": 6,
            "ttr": 0.2727,
            "avgCPT": {
              "amount": "0.1583",
              "currency": "USD"
            },
            "avgCPM": {
              "amount": "2500",
              "currency": "USD"
            },            
            "localSpend": {
              "amount": "0.95",
              "currency": "USD"
            },         
            "totalInstalls": 10,
            "totalNewDownloads": 3,
            "totalRedownloads": 7,
            "viewInstalls": 18,
            "tapInstalls": 5,
            "tapNewDownloads": 2,
            "tapRedownloads": 3,
            "viewNewDownloads": 0,
            "viewReDownloads": 5,
            "totalAvgCPI": {
              "amount": "1.57",
              "currency": "USD"
           },
            "totalInstallRate": 0.962,
            "tapInstallCPI": {
              "amount": "0.19",
              "currency": "USD"
            },
            “tapInstallRate”: 0.8333,
            "date": "2024-04-08"
          },
          {
            "impressions": 15,
            "taps": 7,
            "ttr": 0.4667,
            "avgCPT": {
              "amount": "0.1829",
              "currency": "USD"
            },
            "avgCPM": {
              "amount": "2500",
              "currency": "USD"
            },
            "localSpend": {
              "amount": "1.28",
              "currency": "USD"
            },
            "totalInstalls": 6,
            "totalNewDownloads": 3,
            "totalRedownloads": 7,
            "viewInstalls": 9,
            "tapInstalls": 5,
            "tapNewDownloads": 2,
            "tapRedownloads": 3,
            "viewNewDownloads": 0,
            "viewReDownloads": 5,
            "totalAvgCPI": {
              "amount": "1.57",
              "currency": "USD"
           },
            “totalInstallRate”: 0.962,            
            "tapInstallCPI": {
              "amount": "0.2133",
              "currency": "USD"
            },                     
            "tapInstallRate": 0.8571,
            "date": "2024-04-08"
          }
        ],
        "metadata": {
          "adChannelType": "SEARCH",
          "billingEvent": "TAPS",
          "supplySources": [
            "APPSTORE_SEARCH_RESULTS"
          ],
          "campaignId": 542370539,
          "campaignName": "campaign name example",
          "deleted": false,
          "campaignStatus": "ENABLED",
          "app": {
            "appName": "Trip Trek example app name",
            "adamId": 427916203
          },
          "servingStatus": "RUNNING",
          "servingStateReasons": null,
          "countriesOrRegions": [
            "US"
          ],
          "modificationTime": "2024-04-08T15:51:14.500",
          "totalBudget": {
            "amount": "10000",
            "currency": "USD"
          },
          "dailyBudgetAmount": {
            "amount": "500",
            "currency": "USD"
          },
          "displayStatus": "RUNNING",
          "orgId": 40669820,
          "countryOrRegionServingStateReasons": {},
          "countryOrRegion": "US",
          "deviceClass": "iPhone"
        }
      }
    ]
  }
```

### Payload example 2: Get campaign-level reports

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/reports/campaigns

{
  "startTime": "2024-04-08",
  "endTime": "2024-04-09",
  "selector": {
    "orderBy": [
      {
        "field": "billingEvent",
        "sortOrder": "DESCENDING"
      }
    ],
    "conditions": [
      {
        "field": "billingEvent",
        "operator": "IN",
        "values": [
          "IMPRESSIONS",
          "TAPS"
        ]
      }
    ],
    "pagination": {
      "offset": 0,
      "limit": 34
    }
  },
  "timeZone": "UTC",
  "returnRecordsWithNoMetrics": false,
  "returnRowTotals": true,
  "returnGrandTotals": true
}
```

```
{
      "row": [
        {
          "other": false,
          "total": {
            "impressions": 36,
            "taps": 14,
            "ttr": 4,
            "avgCPT": {
              "amount": "0.625",
              "currency": "USD"
            },
            "avgCPM": {
              "amount": "250",
              "currency": "USD"
            },
            "localSpend": {
              "amount": "900",
              "currency": "USD"
            },
             "totalInstalls": 10,
             "totalNewDownloads": 3,
             "totalRedownloads": 7,
             "viewInstalls": 18,
             "tapInstalls": 5,
            "tapNewDownloads": 10,
            "tapNewDownloads": 10,
            "tapRedownloads": 10,
            "viewNewDownloads": 10,
            "viewReDownloads": 10,
            "totalAvgCPI": {
              "amount": "1.57",
              "currency": "USD"
           },
            "totalInstallRate": 0.962,
            "tapInstallCPI": {
              "amount": "0.8333",
              "currency": "USD"
            },       
           "tapInstallRate": 0.75
          },
          "metadata": {
            "campaignId": 542370539,
            "campaignName": "campaign name example",
            "deleted": false,
            "campaignStatus": "ENABLED",
            "app": {
              "appName": "Trip Trek example app",
              "adamId": 427916203
            },
            "servingStatus": "RUNNING",
            "servingStateReasons": null,
            "countriesOrRegions": [
              "AU",
              "CA",
              "US"
            ],
            "modificationTime": "2024-04-08T09:55:36.265",
            "totalBudget": {
              "amount": "1000",
              "currency": "USD"
            },
            "dailyBudget": 100,
            "displayStatus": "RUNNING",
            "supplySources": [
              "APPSTORE_SEARCH_TAB"
            ],
            "adChannelType": "DISPLAY",
            "orgId": 40669820,
            "countryOrRegionServingStateReasons": {},
            "billingEvent": "IMPRESSIONS"
          }
          }
        ],
        "grandTotals": {
          "other": false,
          "total": {
            "impressions": 74,
            "taps": 29,
            "ttr": 4,
            "avgCPT": {
              "amount": "0.625",
              "currency": "USD"
            },
            "avgCPM": {
              "amount": "250",
              "currency": "USD"
            },
            "localSpend": {
              "amount": "300",
              "currency": "USD"
            },
             "totalInstalls": 10,
             "totalNewDownloads": 3,
             "totalRedownloads": 7,
             "viewInstalls": 18,
             "tapInstalls": 5,
             "tapNewDownloads": 3,
             "tapNewDownloads": 4,
             "tapRedownloads": 8,
             "viewNewDownloads": 12,
             "viewReDownloads": 10,
             "totalAvgCPI": {
              "amount": "1.57",
              "currency": "USD"
           },
             "totalInstallRate": 0.843,
             "tapInstallCPI": {
              "amount": "0.4222",
              "currency": "USD"
            },       
           "tapInstallRate": 0.75
          },
          }
        }
    }
```

### Payload example 3: Get campaign-level reports with granularity

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/reports/campaigns

{  
  "startTime": "2024-04-08",
  "endTime": "2024-04-18",
  "selector": {
    "orderBy": [
      {
        "field": "countryOrRegion",
        "sortOrder": "ASCENDING"
      }
    ],
    "conditions": [
      {
        "field": "countriesOrRegions",
        "operator": "CONTAINS_ANY",
        "values": [
          "US",
          "GB"
        ]
      },
      {
        "field": "countryOrRegion",
        "operator": "IN",
        "values": [
          "US"
        ]
      }
    ],
    "pagination": {
      "offset": 0,
      "limit": 1000
    }
  },
  "groupBy": [
    "countryOrRegion"
  ],
  "timeZone": "UTC",
  "returnRecordsWithNoMetrics": true,
  "returnRowTotals": false,
  "granularity": "DAILY",
  "returnGrandTotals": false
}

```

```
{
    "row": [
      {
        "other": false,
        "granularity": [
          {
            "date": "2024-04-08"
          },
          {
            "date": "2024-04-09"
          },
          {
            "date": "2024-04-10"
          },
          {
            "date": "2024-04-11"
          },
          {
            "date": "2024-04-12"
          },
          {
            "date": "2024-04-13"
          },
          {
            "date": "2024-04-14"
          },
          {
            "date": "2024-04-15"
          },
          {
            "date": "2024-04-16"
          },
          {
            "date": "2021-04-17"
          },
          {
            "date": "2024-04-18"
          }
        ],
        "total": {
           "impressions": 36,
           "taps": 14,
           "ttr": 4,
           "avgCPT": {
             "amount": "0.625",
             "currency": "USD"
            },
            "avgCPM": {
             "amount": "250",
             "currency": "USD”
            },
            "localSpend": {
              "amount": "300",
              "currency": "USD"
            },
             "totalInstalls": 10,
             "totalNewDownloads": 3,
             "totalRedownloads": 7,
             "viewInstalls": 18,
             "tapInstalls": 5,
             "tapNewDownloads": 10,
             "tapNewDownloads": 10,
             "tapRedownloads": 10,
             "viewNewDownloads": 10,
             "viewReDownloads": 10,
             "totalAvgCPI": {
              "amount": "1.57",
              "currency": "USD"
           },
            "totalInstallRate": 0.962,
            "tapInstallCPI": {
              "amount": "0.8333",
              "currency": "USD"
            },       
           "tapInstallRate": 0.75
          },
        "metadata": {
          "billingEvent": "TAPS",
          "supplySources": [
            "APPSTORE_SEARCH_RESULTS"
          ],
          "campaignId": 542370539,
          "campaignName": "Get campaign report name example",
          "deleted": false,
          "campaignStatus": "ENABLED",
          "app": {
            "appName": "Trip Trek example app",
            "adamId": 427916203
          },
          "servingStatus": "RUNNING",
          "servingStateReasons": null,
          "countriesOrRegions": [
            "US"
          ],
          "modificationTime": "2024-04-08T08:46:08.848",
          "totalBudget": {
            "amount": "1000",
            "currency": "USD"
          },
          "dailyBudgetAmount": {
            "amount": "200",
            "currency": "USD"
          },
          "displayStatus": "RUNNING",
          "orgId": 541231618,
          "countryOrRegionServingStateReasons": {},
          "countryOrRegion": "US"
        }
      }
    ]
  }
```

## See Also

### Reports Endpoints

Get Ad Group-Level Reports

Fetches reports for ad groups within a campaign.

Get Keyword-Level Reports

Fetches reports for targeting keywords within a campaign.

Get Keyword-Level within Ad Group Reports

Fetches reports for targeting keywords within an ad group.

Get Search Term-Level Reports

Fetches reports for search terms within a campaign.

Get Search Term-Level within Ad Group Reports

Fetches reports for search terms within an ad group.

Get Ad-Level Reports

Fetches ad performance data within a campaign.

