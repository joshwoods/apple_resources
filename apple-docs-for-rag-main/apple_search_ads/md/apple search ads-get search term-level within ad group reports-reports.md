

- Apple Search Ads
-  Get Search Term-Level within Ad Group Reports 

Web Service Endpoint

# Get Search Term-Level within Ad Group Reports

Fetches reports for search terms within an ad group.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/adgroups/{adgroupId}/searchterms
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

The API can’t locate the resource.

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

Use this endpoint to fetch reports with a high volume of search terms in your campaign. See ReportingSearchTerm for Condition operators and field values to filter results with a Selector.

The limit for search term-level reports is 10 impressions. Search term-level reports only support a `timeZone` value of `ORTZ`. The `orderBy` Selector specifies fields to sort the records list by `ASCENDING` or `DESCENDING`. All ReportingSearchTerm fields are available to the `orderBy` Selector.

### Payload example: Get search term-level within ad group reports

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/adgroups/{adgroupId}/searchterms

{
  "startTime": "2024-04-08",
  "endTime": "2024-04-09",
  "timeZone": "ORTZ",
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
  "groupBy": null
}
```

```
{
      "row": [
        {
          "other": true,
          "total": {
          "impressions": 41,
          "taps": 1,
          "totalInstalls": 1,
          "totalNewDownloads": 2,
          "totalRedownloads": 1,
          "viewInstalls": 1,
          "tapInstalls": 5,
          "tapNewDownloads": 2,
          "tapRedownloads": 3,
          "viewNewDownloads": 6,
          "viewReDownloads": 3,
          "totalInstallRate": 2.962 
          "ttr": 0.0244,
          "tapInstallCPI": {
            "amount": "0",
            "currency": "USD"
            },
          "avgCPT": {
            "amount": "0.88",
            "currency": "USD"
            },
          "localSpend": {
            "amount": "0.88",
            "currency": "USD"
            },
          "tapInstallRate": 0.873,
          "date": "2024-08-10"
          },
          "metadata": {
            "keywordId": 87675434,
            "keyword": "keyword 2",
            "matchType": "EXACT",
            "bidAmount": {
              "amount": "2",
              "currency": "USD"
            },
            "deleted": false,
            "keywordDisplayStatus": "RUNNING",
            "adGroupId": 427916203,
            "adGroupName": "ad group 1",
            "adGroupDeleted": false,
            "searchTermText": null,
            "searchTermSource": "TARGETED"
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

Get Keyword-Level within Ad Group Reports

Fetches reports for targeting keywords within an ad group.

Get Search Term-Level Reports

Fetches reports for search terms within a campaign.

Get Ad-Level Reports

Fetches ad performance data within a campaign.

