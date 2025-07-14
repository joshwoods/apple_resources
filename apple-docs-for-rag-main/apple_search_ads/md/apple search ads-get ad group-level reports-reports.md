

- Apple Search Ads
-  Get Ad Group-Level Reports 

Web Service Endpoint

# Get Ad Group-Level Reports

Fetches reports for ad groups within a campaign.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/adgroups
```

## Path Parameters

`campaignId`

`int64`

 (Required) 

The unique identifier for the campaign.

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

Use this endpoint to fetch reports for your ad groups in campaigns. See ReportingAdGroup for Condition operators and field values to filter results with an object Selector. See the `groupBy` parameter description in the ReportingRequest for supported values per targeting dimension. The `orderBy` Selector specifies fields to sort the records list by `ASCENDING` or `DESCENDING`. All ReportingAdGroup fields are available to the `orderBy` Selector except `adGroupServingStateReasons`.

### Payload example 1: Ad group-level reports

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/adgroups

{
  "startTime": "2024-04-08",
  "endTime": "2024-04-09",
  "selector": {
    "orderBy": [
      {
        "field": "deviceClass",
        "sortOrder": "ASCENDING"
      }
    ],
    "conditions": [
      {
        "field": "deviceClass",
        "operator": "CONTAINS_ANY",
        "values": [
          "IPAD",
          "IPHONE"
        ]
      },
      {
        "field": "ageRange",
        "operator": "IN",
        "values": [
          "18-24",
          "25-34",
          "35-44",
          "45-54"
        ]
      }
    ],
    "pagination": {
      "offset": 0,
      "limit": 1000
    }
  },
  "groupBy": [
    "deviceClass",
    "ageRange"
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
            "impressions": 210,
            "taps": 30,
            "ttr": 0.1429,
            "avgCPT": {
              "amount": "0.3783",
              "currency": "USD"
            },
            "avgCPM": {
              "amount": "0.2500",
              "currency": "USD"
            },
            "localSpend": {
              "amount": "11.35",
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
              "amount": "0.5974",
              "currency": "USD"
            },
           "date": "2024-04-08"
          },
          {
            "impressions": 198,
            "taps": 31,
            "ttr": 0.652,
            "avgCPT": {
              "amount": "0.83",
              "currency": "USD"
            },
            "avgCPM": {
              "amount": "0.2500",
              "currency": "USD"
            },
            "localSpend": {
              "amount": "11.35",
              "currency": "USD"
            },
            "totalInstalls": 13,
            "totalNewDownloads": 3,
            "totalRedownloads": 7,
            "viewInstalls": 18,
            "tapInstalls": 5,
            "tapNewDownloads": 2,
            "tapRedownloads": 3,
            "viewNewDownloads": 2,
            "viewReDownloads": 5,
            "totalAvgCPI": {
              "amount": "1.76",
              "currency": "USD"
           },
            "totalInstallRate": 0.54,
            "tapInstallCPI": {
              "amount": "0.74",
              "currency": "USD"
            },
            "tapInstallRate": 0.76,
            "date": "2024-05-08"
          },
          {
            "impressions": 236,
            "taps": 29,
            "ttr": 0.1229,
            "avgCPT": {
              "amount": "0.4231",
              "currency": "USD"
            },
            "avgCPM": {
              "amount": "0.2500",
              "currency": "USD"
            },
            "localSpend": {
              "amount": "12.27",
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
            "totalInstallRate": 0.962 
            "tapInstallCPI": {
              "amount": "0.4908",
              "currency": "USD"
            },
           "tapInstallRate": 0.91,
            "date": "2024-04-08"
          }
        ],
        "metadata": {
          "adGroupId": 427916204,
          "adGroupName": "ad group example name",
          "startTime": "2024-04-08T00:00:00.000",
          "endTime": null,
          "cpaGoal": null,
          "pricingModel": "CPC",
          "defaultBidAmount": {
            "amount": "100",
            "currency": "USD"
          },
          "deleted": false,
          "adGroupStatus": "ENABLED",
          "adGroupServingStatus": "RUNNING",
          "adGroupServingStateReasons": null,
          "modificationTime": "2024-04-08T10:35:50.194",
          "automatedKeywordsOptIn": false,
          "adGroupDisplayStatus": "RUNNING",
          "campaignId": 542370539,
          "orgId": 40669820,
          "countryOrRegion": "US",
          "deviceClass": "iPhone"
        }
      }
    ]
  }
```

### Payload example 2: Ad group-level reports

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/adgroups

{
  "startTime": "2024-04-08",
  "endTime": "2024-04-09",
  "selector": {
    "orderBy": [
      {
        "field": "defaultBidAmount",
        "sortOrder": "DESCENDING"
      }
    ],
    "conditions": [
      {
        "field": "defaultBidAmount",
        "operator": "BETWEEN",
        "values": [
          "99",
          "101"
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
            "impressions": 1200,
            "taps": 800,
            "ttr": 4,
            "avgCPT": {
              "amount": "0.625",
              "currency": "USD"
            },
            "avgCPM": {
              "amount": "2500",
              "currency": "USD"
            },
            "localSpend": {
              "amount": "3000",
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
            "totalInstallRate": 0.962 
            "tapInstallCPI": {
              "amount": "0.8333",
              "currency": "USD"
            },
            "tapInstallRate": 0.91,
            "date": "2024-05-08"
          },
          "metadata": {
            "adGroupId": 427916203,
            "adGroupName": "ad group 2",
            "startTime": "2024-03-15T09:54:59.117",
            "endTime": "2024-09-11T09:54:59.117",
            "cpaGoal": null,
            "deleted": false,
            "adGroupStatus": "ENABLED",
            "adGroupServingStatus": "RUNNING",
            "adGroupServingStateReasons": null,
            "modificationTime": "2024-04-09T09:55:06.098",
            "adGroupDisplayStatus": "RUNNING",
            "campaignId": 542370539,
            "orgId": 40669820,
            "pricingModel": "CPM",
            "defaultBidAmount": {
              "amount": "100",
              "currency": "USD"
            }
          }
        }
      ],
      "grandTotals": {
        "other": false,
        "total": {
            "impressions": 1020,
            "taps": 800,
            "ttr": 4,
            "avgCPT": {
              "amount": "0.625",
              "currency": "USD"
            },
            "avgCPM": {
              "amount": "2500",
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
            "tapNewDownloads": 2,
            "tapRedownloads": 3,
            "viewNewDownloads": 0,
            "viewReDownloads": 5,
            "totalAvgCPI": {
              "amount": "1.57",
              "currency": "USD"
           },
            "totalInstallRate": 0.962 
            "tapInstallCPI": {
              "amount": "0.8333",
              "currency": "USD"
            },
            "tapInstallRate": 0.76,
            “date”: “2024-05-09”
          },        }
      }
  }
```

## See Also

### Reports Endpoints

Get Campaign-Level Reports

Fetches reports for campaigns.

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

