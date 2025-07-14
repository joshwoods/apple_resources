

- App Store Connect API
-  Read reports for a specific request 

Web Service Endpoint

# Read reports for a specific request

Get a list of reports generated from a specific analytics report request.

App Store Connect API 3.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/{id}/reports
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the Read report requests response.

## Query Parameters

`fields[analyticsReports]`

`[string]`

Possible Values: `name, category, instances`

`filter[category]`

`[string]`

Possible values:

`APP_USAGE`  
A string representing the App Usage category.

`APP_STORE_ENGAGEMENT`  
A string representing the App Store Engagement category.

`COMMERCE`  
A string representing the App Store Commerce category.

`FRAMEWORK_USAGE`  
A string representing the Framework Usage category.

`PERFORMANCE`  
A string representing the Performance category.

Possible Values: `APP_USAGE, APP_STORE_ENGAGEMENT, COMMERCE, FRAMEWORK_USAGE, PERFORMANCE`

`filter[name]`

`[string]`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

AnalyticsReportsResponse

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
GET https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231/reports?limit=5
```

```
{
  "data": [
    {
      "type": "analyticsReports",
      "id": "r19-d48c69c5-9bcb-4592-abbd-08a9411b0231",
      "attributes": {
        "name": "Streaming Playback Performance",
        "category": "PERFORMANCE"
      },
      "relationships": {
        "instances": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r19-d48c69c5-9bcb-4592-abbd-08a9411b0231/relationships/instances",
            "related": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r19-d48c69c5-9bcb-4592-abbd-08a9411b0231/instances"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r19-d48c69c5-9bcb-4592-abbd-08a9411b0231"
      }
    },
    {
      "type": "analyticsReports",
      "id": "r20-d48c69c5-9bcb-4592-abbd-08a9411b0231",
      "attributes": {
        "name": "Streaming Downloads Performance",
        "category": "PERFORMANCE"
      },
      "relationships": {
        "instances": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r20-d48c69c5-9bcb-4592-abbd-08a9411b0231/relationships/instances",
            "related": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r20-d48c69c5-9bcb-4592-abbd-08a9411b0231/instances"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r20-d48c69c5-9bcb-4592-abbd-08a9411b0231"
      }
    },
    {
      "type": "analyticsReports",
      "id": "r142-d48c69c5-9bcb-4592-abbd-08a9411b0231",
      "attributes": {
        "name": "App Crashes Expanded",
        "category": "PERFORMANCE"
      },
      "relationships": {
        "instances": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r142-d48c69c5-9bcb-4592-abbd-08a9411b0231/relationships/instances",
            "related": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r142-d48c69c5-9bcb-4592-abbd-08a9411b0231/instances"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r142-d48c69c5-9bcb-4592-abbd-08a9411b0231"
      }
    },
    {
      "type": "analyticsReports",
      "id": "r143-d48c69c5-9bcb-4592-abbd-08a9411b0231",
      "attributes": {
        "name": "App Storage Reads and Writes",
        "category": "PERFORMANCE"
      },
      "relationships": {
        "instances": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r143-d48c69c5-9bcb-4592-abbd-08a9411b0231/relationships/instances",
            "related": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r143-d48c69c5-9bcb-4592-abbd-08a9411b0231/instances"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r143-d48c69c5-9bcb-4592-abbd-08a9411b0231"
      }
    },
    {
      "type": "analyticsReports",
      "id": "r23-d48c69c5-9bcb-4592-abbd-08a9411b0231",
      "attributes": {
        "name": "AirPlay Performance",
        "category": "PERFORMANCE"
      },
      "relationships": {
        "instances": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r23-d48c69c5-9bcb-4592-abbd-08a9411b0231/relationships/instances",
            "related": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r23-d48c69c5-9bcb-4592-abbd-08a9411b0231/instances"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/analyticsReports/r23-d48c69c5-9bcb-4592-abbd-08a9411b0231"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231/reports?limit=5",
    "next": "https://api.appstoreconnect.apple.com/v1/analyticsReportRequests/d48c69c5-9bcb-4592-abbd-08a9411b0231/reports?cursor=BQ.ALHoGBE&limit=5"
  },
  "meta": {
    "paging": {
      "total": 116,
      "limit": 5
    }
  }
}
```

## See Also

### Making, Reading, and Deleting Requests

Request reports

Request analytics reports for your apps.

Read report requests

Read analytics report requests for a specific app.

Read report request information

Get details for and the state of a specific analytics report request.

Delete a report request

Remove a specific analytics report request.

