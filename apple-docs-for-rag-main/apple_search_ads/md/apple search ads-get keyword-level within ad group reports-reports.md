

- Apple Search Ads
-  Get Keyword-Level within Ad Group Reports 

Web Service Endpoint

# Get Keyword-Level within Ad Group Reports

Fetches reports for targeting keywords within an ad group.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/adgroups/{adgroupId}/keywords
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

ErrorResponseBody

`Bad Request`

An invalid query or missing required parameters.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponseBody

`Not Found`

An unauthenticated call fails to get the requested response.

Content-Type: application/json

` 429 `

ApiErrorResponse

The API calls exceed rate-limit thresholds. See the Rate Limits subsection of Calling the Apple Search Ads API.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorResponseBody

`Internal Server Error`

The Apple Search Ads server is temporarily down or unreachable. The request may be valid, but you need to retry it later.

Content-Type: application/json

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

Use this endpoint to fetch reports for a high volume of targeting keywords in your campaigns. See ReportingKeyword for Condition operators and field values to filter results with a Selector. The `orderBy` Selector specifies fields to sort the records list by `ASCENDING` or `DESCENDING`. All ReportingKeyword fields are available to the `orderBy` Selector.

### Payload example: Get keyword-level within ad group reports

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/adgroups/{adgroupId}/keywords

{
  "startTime": "2024-04-08",
  "endTime": "2024-04-09",
  "timeZone": "UTC",
  "returnRowTotals": true,
  "returnGrandTotals": true,
  "returnRecordsWithNoMetrics": false,
  "selector": {
    "orderBy": [
      {
        "field": "localSpend",
        "sortOrder": "DESCENDING"
      }
    ],
    "conditions": [],
    "pagination": {
      "offset": null,
      "limit": null
    }
  },
  "groupBy" null
}

```

```
{
    "row": [
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
          "amount": "0",
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
          "currency": “USD”
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
              "amount": "400",
              "currency": "USD"
           },
          "suggestedBidAmount": {
            "amount": "2.40",
            "currency": "USD"
             }
        }
      }
    }
  ]
}
```

## See Also

### Reports Endpoints

Get Campaign-Level Reports

Fetches reports for campaigns.

Get Ad Group-Level Reports

Fetches reports for ad groups within a campaign.

Get Keyword-Level Reports

Fetches reports for targeting keywords within a campaign.

Get Search Term-Level Reports

Fetches reports for search terms within a campaign.

Get Search Term-Level within Ad Group Reports

Fetches reports for search terms within an ad group.

Get Ad-Level Reports

Fetches ad performance data within a campaign.

