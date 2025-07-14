

- App Store Connect API
-  Get the Build ID for an App Store Version 

Web Service Endpoint

# Get the Build ID for an App Store Version

Get the ID of the build that is attached to a specific App Store version.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/relationships/build
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 200 ``OK`

AppStoreVersionBuildLinkageResponse

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

## See Also

### Attaching a Build to a Version

Read the Build Information of an App Store Version

Get the build that is attached to a specific App Store version.

Modify the Build for an App Store Version

Change the build that is attached to a specific App Store version.

