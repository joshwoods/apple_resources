

- App Store Connect API
-  Read report request information 

Web Service Endpoint

# Read report request information

Get details for and the state of a specific analytics report request.

App Store Connect API 3.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the Read report requests response.

## Query Parameters

`fields[analyticsReportRequests]`

`[string]`

Possible Values: `accessType, stoppedDueToInactivity, reports`

`fields[analyticsReports]`

`[string]`

Possible Values: `name, category, instances`

`include`

`[string]`

Value: `reports`

`limit[reports]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AnalyticsReportRequestResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## Mentioned in 

Downloading Analytics Reports

## Discussion

Note

If you don’t retrieve data for a long time, a report request changes to `stoppedDueToInactivity`. You need to make a new request to resume getting reports.

### Examples Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231
```

```
{
  "data": {
    "type": "analyticsReportRequests",
    "id": "d48c69c5-9bcb-4592-abbd-08a9411b0231",
    "attributes": {
      "accessType": "ONGOING",
      "stoppedDueToInactivity": false
    },
    "relationships": {
      "reports": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231/relationships/reports",
          "related": "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231/reports"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231"
  }
}
```

## See Also

### Making, Reading, and Deleting Requests

Request reports

Request analytics reports for your apps.

Read report requests

Read analytics report requests for a specific app.

Read reports for a specific request

Get a list of reports generated from a specific analytics report request.

Delete a report request

Remove a specific analytics report request.

