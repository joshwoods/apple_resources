

- Apple Search Ads
-  Get Keyword-Level Reports 

Web Service Endpoint

# Get Keyword-Level Reports

Fetches reports for targeting keywords within a campaign.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/keywords
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

If the call succeeds, the API returns the ReportingResponse object in the response payload with an HTTP status code of `200 (OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Apple Search Ads Campaign Management API 3

## Discussion

Use this endpoint to fetch reports for targeting keywords in your campaigns. See ReportingKeyword for Condition operators and field values to filter results with a Selector.

The `orderBy` Selector specifies fields to sort the records list by `ASCENDING` or `DESCENDING`. All ReportingKeyword fields are available to the `orderBy` Selector.

### Payload example: Get keyword-level reports

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/keywords

{
  "returnRowTotals": true,
  "granularity": "DAILY",
  "timeZone": "UTC",
  "returnGrandTotals": true,
  "startTime": "2024-04-08",
  "selector": {
    "orderBy": [
      {
        "field": "localSpend",
        "sortOrder": "ASCENDING"
      }
    ],
    "conditions": [
      {
        "field": "deleted",
        "operator": "IN",
        "values": [
          "false",
          "true"
        ]
      }
    ],
    "pagination": {
      "offset": 0,
      "limit": 1000
    }
  },
  "endTime": "2024-04-09",
  "returnRecordsWithNoMetrics": true
}
```

```
{
  "row": [
    {
      "other": false,
      "total": {
        "impressions": 76,
        "taps": 45,
        "ttr": 0.45,
        "avgCPT": {
          "amount": “0”,
          "currency": “USD”
        },
        "avgCPM": {
          “amount”: “0”,
          “currency”: “USD”
        },
        "localSpend": {
          "amount": "0",
          "currency":"USD"
        },
        "totalInstalls": 16,
        "totalNewDownloads": 23,
        "totalRedownloads": 17,
        "viewInstalls": 18,
        "tapInstalls": 59,
        "tapNewDownloads": 22,
        "tapRedownloads": 35,
        "viewNewDownloads": 67,
        "viewReDownloads": 53,
        "totalAvgCPI": {
           "amount": "1.57",
           "currency": "USD"
           },
        "totalInstallRate": 2.962
        "tapInstallCPI": {
          "amount": "0",
          "currency": "USD"
        },
       "tapInstallRate": 0.8571,
       "date": "2024-05-08"
      },
      "metadata": {
        "keywordId": 87675432,
        "keyword": "keyword 1",
        "keywordStatus": "ACTIVE",
        "matchType": "BROAD",
        "bidAmount": {
          "amount": "100",
          "currency": "USD"
        },
        "deleted": false,
        "keywordDisplayStatus": "RUNNING",
        "adGroupId": 542317095,
        "adGroupName": "Ad Group 1",
        "adGroupDeleted": false,
        "modificationTime": "2024-04-08T09:33:45.387"
      },
      "insights": {
        "bidRecommendation": {
          "bidMin": {
            "amount": "null",
            "currency": "null"
          },
          "bidMax": {
            "amount": "null",
            "currency": "null"
          },
          "suggestedBidAmount": {
            "amount": "2.40",
            "currency": "USD"
          }
        }
      }
    },
    {
      "other": false,
      "total": {
        "impressions": 53,
        "taps": 45,
        "ttr": 0.45,
        "avgCPT": {
          "amount": "0",
          "currency": "USD"
        },
        "avgCPM": {
          "amount": “0”,
          "currency": "USD"
        },
        "localSpend": {
          "amount": "0",
          "currency":"USD"
        },
        "totalInstalls": 16,
        "totalNewDownloads": 23,
        "totalRedownloads": 17,
        "viewInstalls": 18,
        "tapInstalls": 59,
        "tapNewDownloads": 22,
        "tapRedownloads": 35,
        "viewNewDownloads": 67,
        "viewReDownloads": 53,
        "totalAvgCPI": {
           "amount": "1.57",
           "currency": "USD"
           },
        "totalInstallRate": 2.962
        "tapInstallCPI": {
          "amount": "0",
          "currency": "USD"
        },
       "tapInstallRate": 0.7654,
       "date": "2024-05-08"
      },
       "metadata": {
        "keywordId": 87675432,
        "keyword": "keyword 1",
        "keywordStatus": "ACTIVE",
        "matchType": "BROAD",
        "bidAmount": {
          "amount": "100",
          "currency": "USD"
        },
        "deleted": false,
        "keywordDisplayStatus": "RUNNING",
        "adGroupId": 300452963,
        "adGroupName": "Ad Group 2",
        "adGroupDeleted": false,
        "modificationTime": "2024-04-10T09:33:50.668"
      },
      "insights": {
        "bidRecommendation": {
          "bidMin": null,
          "bidMax": null,
          "suggestedBidAmount": {
            "amount": "2.40",
            "currency": "USD"
          }
        }
      }
    }
  ],
  "grandTotals": {
    "other": false,
    "total": {
       "impressions": 53,
        "taps": 45,
        "ttr": 0.45,
        "avgCPT": {
          "amount": "0",
          "currency": "USD"
        },
        “avgCPM”: {
          "amount": "0",
          "currency": "USD"
        },
        “localSpend”: {
          "amount": "0",
          "currency":"USD"
        },
        "totalInstalls": 16,
        "totalNewDownloads": 23,
        "totalRedownloads": 17,
        "viewInstalls": 18,
        "tapInstalls": 59,
        "tapNewDownloads": 22,
        "tapRedownloads": 35,
        "viewNewDownloads": 67,
        "viewReDownloads": 53,
        "totalAvgCPI": {
           "amount": "1.57",
           "currency": "USD"
           },
        "totalInstallRate": 2.962
        "tapInstallCPI": {
          "amount": "0",
          "currency": "USD"
        },
       "tapInstallRate": 0.7654,
       "date": "2024-05-10"
      },
     }
  }
}
```

## See Also

### Reports Endpoints

Get Campaign-Level Reports

Fetches reports for campaigns.

Get Ad Group-Level Reports

Fetches reports for ad groups within a campaign.

Get Keyword-Level within Ad Group Reports

Fetches reports for targeting keywords within an ad group.

Get Search Term-Level Reports

Fetches reports for search terms within a campaign.

Get Search Term-Level within Ad Group Reports

Fetches reports for search terms within an ad group.

Get Ad-Level Reports

Fetches ad performance data within a campaign.

