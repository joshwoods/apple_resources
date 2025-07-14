

- App Store Connect API
-  Get the Default App Clip Experiences Resource ID for an App Store Version 

Web Service Endpoint

# Get the Default App Clip Experiences Resource ID for an App Store Version

Get the ID of an app’s related default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/relationships/appClipDefaultExperience
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Store Versions resource.

## Response Codes

` 200 ``OK`

AppStoreVersionAppClipDefaultExperienceLinkageResponse

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

## See Also

### Attaching a Default App Clip Experience to a Version

Get the Default App Clip Experience for an App Store Version

Get the default App Clip experience for an App Store version of your app.

Modify the Default App Clip Experience of an App Store Version

Update the relationship between an App Store version and a default App Clip experience.

