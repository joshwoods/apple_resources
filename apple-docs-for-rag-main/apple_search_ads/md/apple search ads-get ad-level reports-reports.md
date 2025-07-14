

- Apple Search Ads
-  Get Ad-Level Reports 

Web Service Endpoint

# Get Ad-Level Reports

Fetches ad performance data within a campaign.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/ads
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

Apple Search Ads Campaign Management API 5

Apple Search Ads Campaign Management API 4

## Discussion

Use this endpoint to return performance data for `ads` within your campaigns. The `orderBy` Selector is required in ad-level report requests. See ReportingAd to identify fields you can use with `orderBy`. To filter results, use selector Condition operators and field values that the `ReportingAd` object specifies. You can only perform `GroupBy` on the CountryOrRegion field. See ReportingRequest.

Historical ad-level metrics for the `APPSTORE_SEARCH_TAB` placement from before API version 5.2 release are reported against `adId=-1`. For `APPSTORE_SEARCH_TAB` ad-level metrics after API version 5.2 release, all default product page ads are reported against a new, real `adId` in reporting payloads.

You can map your campaign installations by `adId` through the AdServices attribution framework.

### Payload example: Get ad-level reports

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/reports/campaigns/{campaignId}/ads

{
  "startTime": "2024-10-08",
  "endTime": "2024-10-09",
  "selector": {
  "orderBy": [
      {
        "field": "creativeType",
        "sortOrder": "ASCENDING"
      }
    ],
    "conditions": [
      {
        "field": "adId",
        "operator": "EQUALS",
        "values": [
          "573408745"
        ]
      }
    ],
    "pagination": {
      "offset": 0,
      "limit": 1000
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
          "impressions": 41,
          "taps": 1,
          "totalInstalls": 1,
          "totalNewDownloads": 2,
          "totalRedownloads": 1,
          "viewInstalls": 1,
          "tapInstalls": 5,
          “tapNewDownloads”: 2,
          "tapRedownloads": 3,
          "viewNewDownloads": 6,
          "viewReDownloads": 3,
          "totalInstallRate": 2.962 
          "ttr": 0.0244,
          "tapInstallCPI": {
            “amount”: "0",
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
          "orgId": 39872140,
          "campaignId": 570798765,
          "adGroupId": 427916203,
          "adId": 573408745,
          "productPageId”: 45812c9b-c296-43d3-c6a0-c5a02f74bf6e,
          "language": "English",
          "creativeId": 94895512,
          "adName": "Trip Trek custom product page variation 1",
          "creativeType": "CUSTOM_PRODUCT_PAGE",
          "status": "VALID",
          "displayStatus": "ACTIVE",
          "adServingStateReasons": null,
          "deleted": false,
          "creationTime": "2024-10-08T06:48:22.812Z",
          "modificationTime": "2024-17-09T06:48:22.812Z"
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

Get Search Term-Level within Ad Group Reports

Fetches reports for search terms within an ad group.

