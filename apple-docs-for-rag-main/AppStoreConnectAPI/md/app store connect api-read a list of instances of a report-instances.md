

- App Store Connect API
-  Read a list of instances of a report 

Web Service Endpoint

# Read a list of instances of a report

Read list of all the granularity options for a specific type of analytics report.

App Store Connect API 3.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/analyticsReports/{id}/instances
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the Read reports for a specific request response.

## Query Parameters

`fields[analyticsReportInstances]`

`[string]`

Possible Values: `granularity, processingDate, segments`

`filter[granularity]`

`[string]`

Possible Values: `DAILY, WEEKLY, MONTHLY`

`filter[processingDate]`

`[string]`

Use ISO 8601 YYYY-MM-DD.

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

AnalyticsReportInstancesResponse

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
GET https://api.appstoreconnect.apple.com/v1/analyticsReports/r2-d48c69c5-9bcb-4592-abbd-08a9411b0231/instances?limit=3&filter%5Bgranularity%5D=DAILY
```

```
{
  "data": [
    {
      "type": "analyticsReportInstances",
      "id": "5c43f2fa-aae7-4290-8664-d6551784c508",
      "attributes": {
        "granularity": "DAILY",
        "processingDate": "2024-01-23"
      },
      "relationships": {
        "segments": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/5c43f2fa-aae7-4290-8664-d6551784c508/relationships/segments",
            "related": "https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/5c43f2fa-aae7-4290-8664-d6551784c508/segments"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/5c43f2fa-aae7-4290-8664-d6551784c508"
      }
    },
    {
      "type": "analyticsReportInstances",
      "id": "42b3c667-3d79-47d0-8ee9-775f685a777c",
      "attributes": {
        "granularity": "DAILY",
        "processingDate": "2024-01-24"
      },
      "relationships": {
        "segments": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/42b3c667-3d79-47d0-8ee9-775f685a777c/relationships/segments",
            "related": "https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/42b3c667-3d79-47d0-8ee9-775f685a777c/segments"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportInstances/42b3c667-3d79-47d0-8ee9-775f685a777c"
      }
    },
    {
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
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r2-d48c69c5-9bcb-4592-abbd-08a9411b0231/instances?limit=3&filter%5Bgranularity%5D=DAILY",
    "next": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r2-d48c69c5-9bcb-4592-abbd-08a9411b0231/instances?cursor=Aw.VGkW1w&limit=3&filter%5Bgranularity%5D=DAILY"
  },
  "meta": {
    "paging": {
      "total": 6,
      "limit": 3
    }
  }
}

```

## See Also

### Reading Reports, Instances, and Segments

Read report information

Get details for a specific analytics report.

Read report instance information

Get details for a specific instance of an analytics report.

Read the segments for a report

Get details for a specific analytics report segment.

Read the details for a report segment

Get details and download information for a specific analytics report segment.

