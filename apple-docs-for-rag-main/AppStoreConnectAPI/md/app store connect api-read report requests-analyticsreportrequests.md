

- App Store Connect API
-  Read report requests 

Web Service Endpoint

# Read report requests

Read analytics report requests for a specific app.

App Store Connect API 3.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/analyticsReportRequests
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[analyticsReportRequests]`

`[string]`

Possible Values: `accessType, stoppedDueToInactivity, reports`

`fields[analyticsReports]`

`[string]`

Possible Values: `name, category, instances`

`filter[accessType]`

`[string]`

Possible Values: `ONE_TIME_SNAPSHOT, ONGOING`

`include`

`[string]`

Value: `reports`

`limit`

`integer`

Maximum: `200`

`limit[reports]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AnalyticsReportRequestsResponse

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

### Examples Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/apps/1476097583/analyticsReportRequests
```

```
{
  "data": [
    {
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
    {
      "type": "analyticsReportRequests",
      "id": "A157dd7a-4fe2-479b-8d25-a8e4228c5b81",
      "attributes": {
        "accessType": "ONE_TIME_SNAPSHOT",
        "stoppedDueToInactivity": false
      },
      "relationships": {
        "reports": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/A157dd7a-4fe2-479b-8d25-a8e4228c5b81/relationships/reports",
            "related": "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/A157dd7a-4fe2-479b-8d25-a8e4228c5b81/reports"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/A157dd7a-4fe2-479b-8d25-a8e4228c5b81"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps/389801252/analyticsReportRequests"
  },
  "meta": {
    "paging": {
      "total": 2,
      "limit": 50
    }
  }
}
```

## See Also

### Making, Reading, and Deleting Requests

Request reports

Request analytics reports for your apps.

Read report request information

Get details for and the state of a specific analytics report request.

Read reports for a specific request

Get a list of reports generated from a specific analytics report request.

Delete a report request

Remove a specific analytics report request.

