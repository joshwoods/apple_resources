

- App Store Connect API
-  Read report information 

Web Service Endpoint

# Read report information

Get details for a specific analytics report.

App Store Connect API 3.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/analyticsReports/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the Read reports for a specific request response.

## Query Parameters

`fields[analyticsReports]`

`[string]`

Possible Values: `name, category, instances`

## Response Codes

` 200 ``OK`

AnalyticsReportResponse

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

### Examples Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/analyticsReports/r2-d48c69c5-9bcb-4592-abbd-08a9411b0231
```

```
{
  "data": {
    "type": "analyticsReports",
    "id": "r2-d48c69c5-9bcb-4592-abbd-08a9411b0231",
    "attributes": {
      "name": "App Crashes",
      "category": "APP_USAGE"
    },
    "relationships": {
      "instances": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r2-d48c69c5-9bcb-4592-abbd-08a9411b0231/relationships/instances",
          "related": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r2-d48c69c5-9bcb-4592-abbd-08a9411b0231/instances"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r2-d48c69c5-9bcb-4592-abbd-08a9411b0231"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r2-d48c69c5-9bcb-4592-abbd-08a9411b0231"
  }
}

```

## See Also

### Reading Reports, Instances, and Segments

Read a list of instances of a report

Read list of all the granularity options for a specific type of analytics report.

Read report instance information

Get details for a specific instance of an analytics report.

Read the segments for a report

Get details for a specific analytics report segment.

Read the details for a report segment

Get details and download information for a specific analytics report segment.

