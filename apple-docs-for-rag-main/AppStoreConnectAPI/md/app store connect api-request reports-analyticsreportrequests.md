

- App Store Connect API
-  Request reports 

Web Service Endpoint

# Request reports

Request analytics reports for your apps.

App Store Connect API 3.4+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/analyticsReportRequests
```

## HTTP Body

AnalyticsReportRequestCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AnalyticsReportRequestResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Mentioned in 

Downloading Analytics Reports

## Discussion

When making a request with this endpoint, the `accessType` `ONGOING` is most common and provides current data. This report request generates reports daily for each granularity: daily, weekly, and monthly. Use `ONE_TIME_SNAPSHOT` to get historical data.

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/analyticsReportRequests 
{
  "data": {
    "type": "analyticsReportRequests",
    "attributes": {
          "accessType": "ONGOING"
    },
    "relationships": {
      "app": {
        "data": {
          "type": "apps",
          "id": "1476097583"
        }
      }
    }
  }
}
```

```
{
  "data" : {
    "type" : "analyticsReportRequests",
    "id" : "d48c69c5-9bcb-4592-abbd-08a9411b0231",
    "attributes" : {
      "accessType" : "ONGOING",
      "stoppedDueToInactivity" : false
    },
    "relationships" : {
      "reports" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231/relationships/reports",
          "related" : "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231/reports"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests"
  }
}
```

## See Also

### Making, Reading, and Deleting Requests

Read report requests

Read analytics report requests for a specific app.

Read report request information

Get details for and the state of a specific analytics report request.

Read reports for a specific request

Get a list of reports generated from a specific analytics report request.

Delete a report request

Remove a specific analytics report request.

