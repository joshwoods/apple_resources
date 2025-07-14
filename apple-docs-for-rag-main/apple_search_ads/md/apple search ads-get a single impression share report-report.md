

- Apple Search Ads
-  Get a Single Impression Share Report 

Web Service Endpoint

# Get a Single Impression Share Report

Fetches a single Impression Share report containing metrics and metadata.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/custom-reports/{reportId}
```

## Path Parameters

`reportId`

`int64`

 (Required) 

Use a `reportId` as a resource in the URI.

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

### Payload example: A single Impression Share report

- Request
- Response

```
HTTP GET https://api.searchads.apple.com/api/v5/custom-reports/{reportId}
```

```
{
  "data": {
    "id": 7615231,
    "name": "impression_share_API_report_example_2",
    "startTime": "2024-06-01",
    "endTime": "2024-06-30",
    "granularity": "DAILY",
    "downloadUri": "https://blobstore.apple.com...",
    "dimensions": [
      "appName",
      "adamId",
      "countryOrRegion",
      "searchTerm"
    ],
    "metrics": [
      "lowImpressionShare",
      "highImpressionShare",
      "rank",
      "searchPopularity"
    ],
    "selector": {
      "conditions": [
        {
          "field": "adamId",
          "operator": "IN",
          "values": [
            "1252497129",
            "282614216"
          ]
        },
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
    "state": "COMPLETED",
    "creationTime": "2024-02-07T09:14:46.235",
    "modificationTime": "2024-02-07T09:14:53.173",
    "dateRange": "LAST_2_WEEKS"
  },
  "pagination": null,
  "error": null
}
```

## See Also

### Impression Share Report Endpoints

Impression Share Report

Obtain a report ID.

Get All Impression Share Reports

Fetches all Impression Share reports containing metrics and metadata.

