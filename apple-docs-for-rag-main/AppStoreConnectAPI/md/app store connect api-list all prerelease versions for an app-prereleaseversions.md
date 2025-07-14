

- App Store Connect API
-  List All Prerelease Versions for an App 

Web Service Endpoint

# List All Prerelease Versions for an App

Get a list of prerelease versions associated with a specific app.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/preReleaseVersions
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`fields[preReleaseVersions]`

`[string]`

Fields to return for included related types.

Possible Values: `version, platform, builds, app`

## Response Codes

` 200 ``OK`

PreReleaseVersionsWithoutIncludesResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/6446998023/preReleaseVersions
```

```
{
  "data": [
    {
      "type": "preReleaseVersions",
      "id": "e5cb13d7-d732-4a57-9ef4-a42c612fc5d7",
      "attributes": {
        "version": "2.0",
        "platform": "IOS"
      },
      "relationships": {
        "builds": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/e5cb13d7-d732-4a57-9ef4-a42c612fc5d7/relationships/builds",
            "related": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/e5cb13d7-d732-4a57-9ef4-a42c612fc5d7/builds"
          }
        },
        "app": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/e5cb13d7-d732-4a57-9ef4-a42c612fc5d7/relationships/app",
            "related": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/e5cb13d7-d732-4a57-9ef4-a42c612fc5d7/app"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/e5cb13d7-d732-4a57-9ef4-a42c612fc5d7"
      }
    },
    {
      "type": "preReleaseVersions",
      "id": "152251d9-a47e-4f43-9861-b5027d721fc9",
      "attributes": {
        "version": "1.0",
        "platform": "IOS"
      },
      "relationships": {
        "builds": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/152251d9-a47e-4f43-9861-b5027d721fc9/relationships/builds",
            "related": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/152251d9-a47e-4f43-9861-b5027d721fc9/builds"
          }
        },
        "app": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/152251d9-a47e-4f43-9861-b5027d721fc9/relationships/app",
            "related": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/152251d9-a47e-4f43-9861-b5027d721fc9/app"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/152251d9-a47e-4f43-9861-b5027d721fc9"
      }
    },
    {
      "type": "preReleaseVersions",
      "id": "bf21597c-6deb-4329-9634-7d28b526156b",
      "attributes": {
        "version": "1.1",
        "platform": "IOS"
      },
      "relationships": {
        "builds": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/bf21597c-6deb-4329-9634-7d28b526156b/relationships/builds",
            "related": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/bf21597c-6deb-4329-9634-7d28b526156b/builds"
          }
        },
        "app": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/bf21597c-6deb-4329-9634-7d28b526156b/relationships/app",
            "related": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/bf21597c-6deb-4329-9634-7d28b526156b/app"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/preReleaseVersions/bf21597c-6deb-4329-9634-7d28b526156b"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/preReleaseVersions"
  },
  "meta": {
    "paging": {
      "total": 3,
      "limit": 50
    }
  }
}

```

## See Also

### Getting app build and prerelease version information

List All Builds of an App

Get a list of builds associated with a specific app.

