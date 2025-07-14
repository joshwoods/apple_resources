

- Apple Search Ads
-  Get All Impression Share Reports 

Web Service Endpoint

# Get All Impression Share Reports

Fetches all Impression Share reports containing metrics and metadata.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/custom-reports
```

## Query Parameters

`field`

`string`

The name of a field.

Default: `creationTime`

`limit`

`integer`

The number of items to return per request. For most objects, the default is `20` and the maximum is `50`.

Default: `20`

Minimum: `1`

`offset`

`integer`

The offset pagination that limits the number of returned records. The start of each page is offset by the specified number.

Default: `0`

Minimum: `0`

`sortOrder`

`string`

The order of grouped results.

Default: `DESCENDING`

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

Use this endpoint to return all Impression Share reports containing metrics and metadata. Use query parameters as needed.

The rate limit for this endpoint is 150 reports within 15 minutes.

### Payload example: All Impression Share reports

- Request
- Response

```
HTTP GET https://api.searchads.apple.com/api/v5/custom-reports
```

```
{
  "data": [
    {
      "id": 965992,
      "name": "impression_share_report_example_3",
      "startTime": "2024-10-14",
      "endTime": "2024-11-12",
      "granularity": "DAILY",
      "downloadUri": "http://blobstore.apple.com...",
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
            "field": "countryOrRegion",
            "operator": "IN",
            "values": [
              "US",
              "AU"
            ]
          },
          {
            "field": "adamId",
            "operator": "IN",
            "values": [
              "1252497129",
              "282614216"
            ]
          }
        ]
      },
      "state": "COMPLETED",
      "creationTime": "2024-02-07T09:23:03.532",
      "modificationTime": "2024-02-07T09:23:09.774",
      "dateRange": "LAST_2_WEEKS"
    },
    {
      "id": 16627,
      "name": "impression_share_report_4",
      "startTime": "2024-09-15",
      "endTime": "2024-10-10",
      "granularity": "DAILY",
      "downloadUri": "http://blobstore.apple.com...",
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
            "field": "countryOrRegion",
            "operator": "IN",
            "values": [
              "US",
              "AU"
            ]
          },
          {
            "field": "adamId",
            "operator": "IN",
            "values": [
              "1252497129",
              "282614216"
            ]
          }
        ]
      },
      "state": "COMPLETED",
      "creationTime": "2024-02-07T09:14:46.235",
      "modificationTime": "2024-02-07T09:14:53.173",
      "dateRange": "LAST_2_WEEKS"
    }
  ],
  "pagination": {
    "totalResults": 2,
    "startIndex": 0,
    "itemsPerPage": 2
  },
  "error": null
}
```

## See Also

### Impression Share Report Endpoints

Impression Share Report

Obtain a report ID.

Get a Single Impression Share Report

Fetches a single Impression Share report containing metrics and metadata.

