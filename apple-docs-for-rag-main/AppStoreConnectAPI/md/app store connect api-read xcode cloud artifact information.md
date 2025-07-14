

- App Store Connect API
-  Read Xcode Cloud Artifact Information 

Web Service Endpoint

# Read Xcode Cloud Artifact Information

Get information about the artifact Xcode Cloud created for a specific action when it performed a build.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciArtifacts/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Artifacts resource.

## Query Parameters

`fields[ciArtifacts]`

`[string]`

Additional fields to include for the Artifacts resource returned by the response.

Possible Values: `fileType, fileName, fileSize, downloadUrl`

## Response Codes

` 200 ``OK`

CiArtifactResponse

`OK`

The request completed successfully.

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

The example request below retrieves detailed information about a specific artifact Xcode Cloud created when it performed a build. Use the information provided to download the artifact and store it on your own servers. Note that the returned download URL is only valid for a limited amount of time.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciArtifacts/73be0e4e-6da2-471a-b652-47bd99885dbc
```

```
{    
"data": {
        "type": "ciArtifacts",
        "id": "73be0e4e-6da2-471a-b652-47bd99885dbc",
        "attributes": {
            "fileType": "LOG_BUNDLE",
            "fileName": "exampleName",
            "fileSize": 19,
            "downloadUrl": "https://example.com/url-to-artifact"
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/ciArtifacts/73be0e4e-6da2-471a-b652-47bd99885dbc"
        }
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciArtifacts/73be0e4e-6da2-471a-b652-47bd99885dbc"
    }
}

```

