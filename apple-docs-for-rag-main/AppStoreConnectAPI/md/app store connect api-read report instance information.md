

- App Store Connect API
-  Read report instance information 

Web Service Endpoint

# Read report instance information

Get details for a specific instance of an analytics report.

App Store Connect API 3.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the Read a list of instances of a report response.

## Query Parameters

`fields[analyticsReportInstances]`

`[string]`

Possible Values: `granularity, processingDate, segments`

## Response Codes

` 200 ``OK`

AnalyticsReportInstanceResponse

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

## Discussion

Note

If you don’t retrieve data for a long time, a report request changes to `stoppedDueToInactivity`. You need to make a new request to resume getting reports.

### Examples Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/d4a141c8-7647-4bdf-b9ae-04cab705d641
```

```
{
  "data": {
    "type": "analyticsReportInstances",
    "id": "d4a141c8-7647-4bdf-b9ae-04cab705d641",
    "attributes": {
      "granularity": "DAILY",
      "processingDate": "2024-01-25"
    },
    "relationships": {
      "segments": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/d4a141c8-7647-4bdf-b9ae-04cab705d641/relationships/segments",
          "related": "https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/d4a141c8-7647-4bdf-b9ae-04cab705d641/segments"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/d4a141c8-7647-4bdf-b9ae-04cab705d641"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/d4a141c8-7647-4bdf-b9ae-04cab705d641"
  }
}

```

## See Also

### Reading Reports, Instances, and Segments

Read report information

Get details for a specific analytics report.

Read a list of instances of a report

Read list of all the granularity options for a specific type of analytics report.

Read the segments for a report

Get details for a specific analytics report segment.

Read the details for a report segment

Get details and download information for a specific analytics report segment.

