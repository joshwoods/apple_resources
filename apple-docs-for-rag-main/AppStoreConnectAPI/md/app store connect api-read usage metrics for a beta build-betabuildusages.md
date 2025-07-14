

- App Store Connect API
-  Read usage metrics for a beta build 

Web Service Endpoint

# Read usage metrics for a beta build

Get usage metrics for a specific build.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/builds/{id}/metrics/betaBuildUsages
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the build resource ID from the List Builds response.

## Query Parameters

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

BetaBuildUsagesV1MetricResponse

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

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/builds/ace4f47a-60ae-4ed6-954f-c4e61c7baab0/metrics/betaBuildUsages
```

```
{
  “data”: [
    {
      “type”: “betaBuildUsages”,
      “dataPoints”: [
        {
          “start”: “2022-10-05”,
          “end”: “2023-10-05”,
          “values”: {
            “installCount”: 2,
            “crashCount”: 0,
            “sessionCount”: 0,
            “inviteCount”: 0,
            “feedbackCount”: 0
          }
        }
      ]
    }
  ],
  “links”: {
    “self”: “https://api.appstoreconnect.apple.com/v1/builds/ace4f47a-60ae-4ed6-954f-c4e61c7baab0/metrics/betaBuildUsages”
  },
  “meta”: {
    “paging”: {
      “total”: 1,
      “limit”: 50
    }
  }
}

```

## See Also

### Getting Build Information

List Builds

Find and list builds for all apps in App Store Connect.

Read Build Information

Get information about a specific build.

Read the App Information of a Build

Get the app information for a specific build.

Read the App Store Version Information of a Build

Get the App Store version of a specific build.

Read the Prerelease Version of a Build

Get the prerelease version for a specific build.

