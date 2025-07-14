

- Apple Search Ads
-  Impression Share Report 

Web Service Endpoint

# Impression Share Report

Obtain a report ID.

Search Ads 5.0+

## URL

``` source
POST https://api.searchads.apple.com/api/v5/custom-reports
```

## HTTP Body

CustomReportRequest

The impression share report request body, consisting of metrics and dimensions to filter on.

Content-Type: application/json

## Response Codes

` 200 ``OK`

CustomReportResponseBody

`OK`

If the call succeeds, the API returns the CustomReportResponseBody object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

Use this endpoint to obtain a `reportId` to use in a Get a Single Impression Share Report request. This endopoint supports selectors. See CustomReportRequest for selector structure.

- You can generate up to 10 reports within 24 hours.

- You can create reports for a range of up to 30 days for any time period after `2020-04-12`.

- You can’t edit or remove report fields.

- Impression Share reports with a `WEEKLY` granularity value can’t have custom `startTime` and `endTime` in the request payload. Use `dateRange` instead. See CustomReportRequest.

### Payload example: Obtain a report ID

- Request
- Response

```
POST https://api.searchads.apple.com/api/v5/custom-reports

{
  "name": "impression_share_API_report_example_1",
  "startTime": "2024-01-20",
  "endTime": "2024-01-29",
  "granularity": "DAILY",
  "selector": {
    "conditions": [
      {
        "field": "countryOrRegion",
        "operator": "IN",
        "values": [
          "US",
          "AU"
        ]
      }
    ]
  }
}
```

```
{
  "data": {
    "id": 986235,
    "name": "impression_share_API_report_example_1",
    "startTime": "2024-01-20",
    "endTime": "2024-01-29",
    "granularity": "DAILY",
    "downloadUri": "https://blobstore.apple.com...",
    "dimensions": [
      "appName",
      "adamId",
      "countryOrRegion",
      "searchTerm"
    ],
    “metrics”: [
      "lowImpressionShare",
      "highImpressionShare",
      "rank",
      "searchPopularity"
    ],
    "selector": {
      "conditions": [
        {
          "field": "countryOrRegion",
          "operator": "IN",
          "values": [
            "US",
            "AU"
          ]
        }
      ]
    },
    "state": "QUEUED",
    "creationTime": "2024-01-12T04:47:27.782",
    "modificationTime": "2024-01-12T04:47:27.782"
  },
  "pagination": null,
  "error": null
}
```

## See Also

### Impression Share Report Endpoints

Get a Single Impression Share Report

Fetches a single Impression Share report containing metrics and metadata.

Get All Impression Share Reports

Fetches all Impression Share reports containing metrics and metadata.

